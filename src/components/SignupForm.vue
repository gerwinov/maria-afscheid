<template>
  <div>
    <div class="alert alert-success alert-dismissible" v-show="success">
      Bedankt voor je aanmelding!
      <button type="button" class="close" aria-label="Close" @click="success = false">
        <span aria-hidden="true">&times;</span>
      </button>
    </div>

    <div class="alert alert-danger alert-dismissible" v-show="error">
      {{ errorMessage }}
      <button type="button" class="close" aria-label="Close" @click="error = false">
        <span aria-hidden="true">&times;</span>
      </button>
    </div>

    <div id="formulier" v-if="formtonen">
    <form novalidate="true">
      <div class="form-group">
        <label for="name">Naam</label>
        <input id="name" class="form-control flex-fill mr-0 mr-sm-2 mb-3 mb-sm-0" :class="{'is-invalid' : formErrors.naam}" type="text" placeholder="Voor- en achternaam" v-model="form.naam" @input="delete formErrors.naam">
        <p class="invalid-feedback" v-show="formErrors.naam">{{ formErrors.naam }}</p>
      </div>

      <div class="form-group">
        <label for="email">E-mailadres</label>
        <input id="email" class="form-control" :class="{'is-invalid' : formErrors.email}" type="text" placeholder="Op dit mailadres ontvang je een bevestiging" v-model="form.email" @input="delete formErrors.email">
        <p class="invalid-feedback" v-show="formErrors.email">{{ formErrors.email }}</p>
      </div>

      <div class="form-group">
        <label for="aanwezigheid">Ik meld me aan voor</label>
        <select id="aanwezigheid" class="form-control" v-model="form.aanwezigheid" :class="{'is-invalid' : formErrors.aanwezigheid}">
          <option>Het hele programma</option>
          <option>Alleen de receptie</option>
        </select>
        <p class="invalid-feedback" v-show="formErrors.aanwezigheid">{{ formErrors.aanwezigheid }}</p>
      </div>

      <div class="form-group">
        <label for="opmerkingen">Jouw boodschap voor Maria (optioneel)</label>
        <textarea class="form-control" id="opmerkingen" placeholder="Wat wil je Maria nog meegeven?" rows="4" v-model="form.opmerkingen"></textarea>
      </div>

      <div class="form-group" >
          <vue-recaptcha :sitekey="captcha.sitekey" @verify="captcha.key = $event; delete formErrors.captcha; captchaError = false" @expired="captcha.key = ''" ref="captcha"></vue-recaptcha>
        <p class="invalid-feedback" :class="{'d-block' : formErrors.captcha }" v-show="captchaError">{{ formErrors.captcha }}</p>
      </div>

      <div class="form-group" >
        <button class="btn btn-primary" @click="submit" :disabled="loading">
          <span class="spinner-border" role="status" aria-hidden="true" v-show="loading"></span>
          Aanmelden
        </button>
      </div>
    </form>
  </div>
  </div>
</template>

<script>
import VueRecaptcha from 'vue-recaptcha'
import { sendXHR } from '../assets/sendXHR'

export default {
  name: 'SignupForm',

  components: { VueRecaptcha },

  mixins: [sendXHR],

  data() {
    return {
      form: {
        naam: null,
        email: null,
        aanwezigheid: 'Het hele programma'
      },
      formErrors: {},
      captcha: {
        sitekey: '6LfHfMkUAAAAAMIr8wPqQubfgNFagnPEOBnuMPy_',
        key: null,
      },
      captchaError: false,
      url: 'https://script.google.com/macros/s/AKfycbyajj9Hg-eHcq3-Ujoc7t2Wgdj6io_cLuRpLN3ojRBP1IPHdQ/exec',
      loading: false,
      success: false,
      error: false,
      errorMessage: null,
      formtonen: true
    }
  },

  methods: {
    submit (e) {
      e.preventDefault();
      
      this.loading = true
      this.formErrors = {}

      if (!this.form.naam) {
        this.formErrors.naam = "Naam is verplicht."
      }
      if (!this.form.aanwezigheid) {
        this.formErrors.aanwezigheid = "Geef aan of je aanwezig bent."
      }
      if (!this.captcha.key) {
        this.formErrors.captcha = "Bevestig dat je geen robot bent."
        this.captchaError = true;
      }
      if (!this.form.email) {
        this.formErrors.email = 'Emailadres is verplicht.'
      } else if (!this.validEmail(this.form.email)) {
        this.formErrors.email = 'Emailadres is ongeldig.'
      }

      if (Object.keys(this.formErrors).length) {
        this.loading = false
        return
      }



      let body = {
        ...this.form, 
        captchaKey: this.captcha.key,
        formGoogleSendEmail: this.form.email
      }

      // Send using XHR
      this.sendXHR('POST', this.url, body)
      this.error = false
    },

    validEmail(email) {
      // eslint-disable-next-line
      var re = /^(([^<>()\[\]\\.,;:\s@"]+(\.[^<>()\[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/
      return re.test(email)
    },

    onSuccess () {
      this.success = true
      this.formtonen = false
      this.loading = false
      this.clear()
      window.location.replace("#contact")

    },

    onError (error) {
      this.loading = this.success = false
      this.errorMessage = error
      this.error = true
    },

    clear () {
      this.errorMessage = null
      for (let key in this.form ) {
        this.form[key] = null
      }      
    }
  }
}
</script>
