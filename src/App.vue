<template>
  <div id="app">
    <!--Preloader div-->
    <div class="preloader"></div>

    <!-- Fixed navbar -->
    <nav class="navbar navbar-default navbar-fixed-top">
        <div class="container">
            <div class="navbar-header">
                <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#navbar" aria-expanded="false" aria-controls="navbar">
                    <span class="sr-only">Toggle navigation</span>
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                </button>
            </div>
            <div id="navbar" class="navbar-collapse collapse">

                <ul class="nav navbar-nav navbar-right">
                    <li class="active"><a href="#top">Start</a></li>
                    <li><a href="#schedule">Programma</a></li>
                    <li><a href="#sponsors">Over Maria</a></li>
                    <li><a href="#venue">Locatie</a></li>
                    <li><a href="#contact">Aanmelden</a></li>
                </ul>
            </div>
            <!--/.nav-collapse -->
        </div>
    </nav>
    <!-- // End Fixed navbar -->

    <header id="top" class="header">
        <div class="container header-container">

            <div class="header_top-bg">
                <div class="logo">
                    
                </div>
            </div>

            <h3 class="headline-support wow fadeInDown">AFSCHEID MARIA SCHUTTE</h3>
            <p class="headline-text wow fadeInDown">Stafarts Centrum Jeugd en Gezin Apeldoorn</p>

            <h1 class="headline wow fadeInDown" data-wow-delay="0.1s">HET KIND EERST</h1>
            <p class="headline-text headline-2 wow fadeInDown">"Elk kind heeft het recht om kind te zijn"</p>
            <p class="headline-text wow fadeInDown">Verdrag Inzake de Rechten van het Kind</p>

            <div class="when_where wow fadeIn" data-wow-delay="0.4s">
                <p class="event_when">24 januari 2020</p>
                <p class="event_where">Proeflokaal De Vlijt, Apeldoorn</p>
            </div>

            <div class="header_bottom-bg">
                <a class="btn btn-default btn-xl wow zoomIn" data-wow-delay="0.3s" href="#contact">AANMELDEN</a>
            </div>

        </div>
        <!-- end .container -->
    </header>
    <!-- end .header -->

    <!-- 
     Highlight Section
     ====================================== -->

    <section class="highlight">

        <div class="container">
            <p class="lead text-center">De jeugdgezondheidszorg in Nederland behoort tot de beste ter wereld. Door alle georganiseer en goede bedoelingen worden organisaties en processen op den duur leidend. Verliezen we dan het belangrijkste niet vaak uit het oog? Het kind zelf heeft het recht om in al ons denken en handelen centraal te staan. Een kleine bijeenkomst om uw gedachten weer op het goede spoor te zetten...</p>

            <div class="countdown_wrap">
                <!-- Countdown JS for the Event Date Starts here.
    TIP: You can change your event time below in the Same Format.  -->

                <ul id="countdown" data-event-date="24 january 2020 16:00:00">
                    <li class="wow zoomIn" data-wow-delay="0s"> <span class="days">00</span>
                        <p class="timeRefDays">days</p>
                    </li>
                    <li class="wow zoomIn" data-wow-delay="0.2s"> <span class="hours">00</span>
                        <p class="timeRefHours">hours</p>
                    </li>
                    <li class="wow zoomIn" data-wow-delay="0.4s"> <span class="minutes">00</span>
                        <p class="timeRefMinutes">minutes</p>
                    </li>
                    <li class="wow zoomIn" data-wow-delay="0.6s"> <span class="seconds">00</span>
                        <p class="timeRefSeconds">seconds</p>
                    </li>
                </ul>
            </div>
            <!-- end .countdown_wrap -->

            <div class="text-center">

                <!-- Add to Calendar Plugin. 
                     For Customization, Visit https://addtocalendar.com/ -->

                <span class="addtocalendar atc-style-theme">
                <a class="atcb-link"><i class="fa fa-calendar"> </i> Voeg toe aan uw agenda</a>
                  <var class="atc_event">
                      <var class="atc_date_start">2020-01-24 16:00:00</var>
                      <var class="atc_date_end">2020-01-24 20:00:00</var>
                      <var class="atc_timezone">Europe/Amsterdam</var>
                      <var class="atc_title">Afscheid Maria Schutte</var>
                      <var class="atc_description"></var>
                      <var class="atc_location">Proeflokaal de Vlijt, Apeldoorn</var>
                  </var>
               </span>

            </div>

        </div>
        <!-- end .container -->

    </section>
    <!-- end section.highlight -->

    <!-- 
     Our Schedule
     ====================================== -->

    <section class="schedule" id="schedule">

        <div class="container">
            <div class="section-title wow fadeInUp">
                <h4>PROGRAMMA</h4>
            </div>

            <!-- Tab panes -->
            <div class="tab-content">
                <div role="tabpanel" class="tab-pane active" id="day1">

                    <!-- ########## Schedule Timeline DAY 01 Starts ########### -->

                    <section class="timeline">
                        <div class="timeline-block">
                            <div class="timeline-bullet wow zoomIn" data-wow-delay="0s">

                            </div>
                            <!-- timeline-bullet -->

                            <div class="timeline-content">
                                <h2 class="wow flipInX" data-wow-delay="0.3s"> Ontvangst met koffie en thee</h2>
                                <p class="wow flipInX" data-wow-delay="0.3s">In proeflokaal De Vlijt</p>
                                <span class="date wow flipInX" data-wow-delay="0.3s">16:00</span>
                            </div>
                            <!-- timeline-content -->
                        </div>
                        <!-- timeline-block -->

                        <div class="timeline-block">
                            <div class="timeline-bullet wow zoomIn" data-wow-delay="0s">

                            </div>
                            <!-- timeline-bullet -->

                            <div class="timeline-content">
                                <h2 class="wow flipInX" data-wow-delay="0.3s"> Start minicongres</h2>
                                <p class="wow flipInX" data-wow-delay="0.3s">In zaal STOOM</p>
                                <div class="speaker-info wow fadeIn" data-wow-delay="0s">
                                    <img src="images/saskia.jpg" alt="avatar" class="img-responsive">
                                </div>
                                <h2 class="wow flipInX" data-wow-delay="0.3s"> Saskia Blom</h2>
                                <p class="wow flipInX" data-wow-delay="0.3s">Opening en inleiding door dagvoorzitter Saskia Blom, directeur Centrum voor Jeugd en Gezin Apeldoorn.</p>
                                <span class="date wow flipInX" data-wow-delay="0.3s">16:30</span>
                            </div>
                            <!-- timeline-content -->
                        </div>
                        <!-- timeline-block -->

                        <div class="timeline-block">
                            <div class="timeline-bullet wow zoomIn" data-wow-delay="0s">

                            </div>
                            <!-- timeline-bullet -->

                            <div class="timeline-content end">
                                <div class="speaker-info wow fadeIn justify-content-end" data-wow-delay="0s">
                                    <img src="images/goos.jpg" alt="avatar" class="img-responsive">
                                </div>
                                <h2 class="wow flipInX" data-wow-delay="0.3s"> Goos Cardol</h2>
                                <p class="wow flipInX" data-wow-delay="0.3s">
                                    <strong>De kunst van het vertalen van het Kinderrechtenverdrag naar de jeugdgezondheidszorg.</strong><br><br>
                                    Goos Cardol leidt het onderzoeksprogramma 'Opvoeden in het publieke domein' op Zuyd Hogeschool en was de afgelopen jaren bijzonder lector van het lectoraat Jeugdzorg. Hij volgde Nederlands Recht aan de Open Universiteit en promoveerde aan de Universiteit Tilburg. Naast zijn functie bij Zuyd is Goos Cardol werkzaam als stafjurist bij de Raad voor de Kinderbescherming. 
                                    <br><i>"Kinderen positie geven. Daar gaat het naar mijn mening om in het internationale kinderrechtenverdrag. Ik prijs me gelukkig dat ik daar mijn steentje aan kan bijdragen."</i>
                                </p>
                                <span class="date wow flipInX" data-wow-delay="0.3s">16:35</span>
                            </div>
                            <!-- timeline-content -->
                        </div>
                        <!-- timeline-block -->

                        <div class="timeline-block">
                            <div class="timeline-bullet wow zoomIn" data-wow-delay="0s">

                            </div>
                            <!-- timeline-bullet -->

                            <div class="timeline-content">
                                <div class="speaker-info wow fadeIn" data-wow-delay="0s">
                                    <img src="images/willemijn.jpg" alt="avatar" class="img-responsive">
                                </div>
                                <h2 class="wow flipInX" data-wow-delay="0.3s"> Willemijn Dupuis</h2>
                                <p class="wow flipInX" data-wow-delay="0.3s">
                                    <strong>Kinderparticipatie begint bij het eigen verhaal van ieder kind.</strong> <br><br>
                                    Willemijn Dupuis is al sinds 1987 bezig met kinderparticipatie in Nederland. Eerst als vrijwilliger bij Unicef, vervolgens als onbezoldigd directeur van de stichting Jeugd NU en tegenwoordig als onbezoldigd directeur van KinderrechtenNU (voornamelijk gericht op kinderen in de leeftijd van negen tot twaalf jaar, ouders en professionals). Met KinderrechtenNU brengt Dupuis kinderrechten onder de aandacht bij gemeenten, professionals, scholen, opvoeders en kinderen.
                                    <br><i>"Kinderen doen n&uacute; mee. Dat betekent nú investeren in l&aacute;ter."</i>
                                </p>
                                <span class="date wow flipInX" data-wow-delay="0.3s">17:00</span>
                            </div>
                            <!-- timeline-content -->
                        </div>
                        <!-- timeline-block -->

                        <div class="timeline-block">
                            <div class="timeline-bullet wow zoomIn" data-wow-delay="0s">

                            </div>
                            <!-- timeline-bullet -->

                            <div class="timeline-content end">
                                <div class="speaker-info wow fadeIn justify-content-end" data-wow-delay="0s">
                                    <img src="images/saskia.jpg" alt="avatar" class="img-responsive">
                                </div>
                                <h2 class="wow flipInX" data-wow-delay="0.3s"> Saskia Blom</h2>
                                <p class="wow flipInX" data-wow-delay="0.3s">Afluisting minicongres door de dagvoorzitter.</p>
                                <span class="date wow flipInX" data-wow-delay="0.3s">17:25</span>
                            </div>
                            <!-- timeline-content -->
                        </div>
                        <!-- timeline-block -->

                        <div class="timeline-block">
                            <div class="timeline-bullet wow zoomIn" data-wow-delay="0s">

                            </div>
                            <!-- timeline-bullet -->

                            <div class="timeline-content">
                                <h2 class="wow flipInX" data-wow-delay="0.3s"> Receptie</h2>
                                <p class="wow flipInX" data-wow-delay="0.3s">Muzikale omlijsting door Steven Schutte, met medewerking van Laura Lijbers</p>
                                <span class="date wow flipInX" data-wow-delay="0.3s">17:30</span>
                            </div>
                            <!-- timeline-content -->
                        </div>
                        <!-- timeline-block -->

                        <div class="timeline-block">
                            <div class="timeline-bullet wow zoomIn" data-wow-delay="0s">

                            </div>
                            <!-- timeline-bullet -->

                            <div class="timeline-content">
                                <h2 class="wow flipInX" data-wow-delay="0.3s"> Rondleiding door de brouwerij</h2>
                                <p class="wow flipInX end" data-wow-delay="0.3s">(optioneel - tijdens de receptie)</p>
                                <span class="date wow flipInX" data-wow-delay="0.3s">17:30</span>
                            </div>
                            <!-- timeline-content -->
                        </div>
                        <!-- timeline-block -->

                        <div class="timeline-block">
                            <div class="timeline-bullet wow zoomIn" data-wow-delay="0s">

                            </div>
                            <!-- timeline-bullet -->

                            <div class="timeline-content">
                                <h2 class="wow flipInX" data-wow-delay="0.3s"> Afsluiting</h2>
                                <span class="date wow flipInX" data-wow-delay="0.3s">20:00</span>
                            </div>
                            <!-- timeline-content -->
                        </div>
                        <!-- timeline-block -->
                    </section>
                    <!-- timeline -->

                    <!-- ########### End Schedule Timeline  DAY 01  ########### -->

                </div>
            </div>

        </div>
        <!-- end .container -->

    </section>
    <!-- end section.schedule -->

    <!-- 
     Our Sponsors
     ====================================== -->

    <section class="sponsors" id="sponsors">

        <div class="container">
            <div class="section-title wow fadeInUp">
                <h4>OVER MARIA</h4>
                <p>Maria (1957) begon haar carrière in de JGZ in 1988 als consultatiebureau-arts voor 2 middagen per week. In 1991 werd ze kostwinner en kon ze haar werkweek maximaal uitbreiden. Alleen consultatiebureaus waren niet genoeg: ze zette zich in voor de ondernemingsraad, voor diverse beroepsorganisaties en deelde haar passie en kennis met anderen als opleider en docent. 
                    <br><br>In 2007 begon ze als pionier de functie van jeugdarts voor alle leeftijdscategorieën te combineren. Vanaf 2011 is ze als stafarts niet alleen inhoudelijk maar ook beleidsmatig met haar beroep bezig, met name op het juridische vlak en in de automatisering. Haar zorgen over het vak zijn consolidering en institutionalisering, haar wensen voor de toekomst van de jeugdgezondheidszorg verdere professionalisering en vernieuwing.</p>
            </div>

            <div class="sponsor-slider wow bounceIn">
                <div><img src="images/photos/1.jpg" class="img-responsive center-block" alt="sponsor"> </div>
                <div><img src="images/photos/2.jpg" class="img-responsive center-block" alt="sponsor"> </div>
                <div><img src="images/photos/3.jpg" class="img-responsive center-block" alt="sponsor"> </div>
                <div><img src="images/photos/4.png" class="img-responsive center-block" alt="sponsor"> </div>
                <div><img src="images/photos/5.png" class="img-responsive center-block" alt="sponsor"> </div>
                <div><img src="images/photos/6.png" class="img-responsive center-block" alt="sponsor"> </div>
                <div><img src="images/photos/0.png" class="img-responsive center-block" alt="sponsor"> </div>
            </div>
        </div>
        <!-- end .container -->
    </section>
    <!-- end section.sponsors -->

    <!-- 
     Contact us
     ====================================== -->

    <div class="highlight highlight-venue" id="venue">
        <div class="container highlight-venue-container">

            <div class="row d-flex-location">
                <div class="col-sm-6 d-flex-location">
                    <div class="contact-box">
                        <img src="images/location-icon.png" alt="location icon" class="wow zoomIn">
                        <h5>LOCATIE</h5>
                        <p>Bierbrouwerij de Vlijt
                            <br>Vlijtseweg 114
                            <br>7317 AG Apeldoorn
                            <br>
                            <br>
                            <a href="https://www.veluwseschavuyt.nl/">Meer over de Veluwse Schavuyt</a>
                        </p>
                    </div>
                </div>
                <div class="col-sm-6 d-flex-location">
                    <div class="contact-box">
                        <h5>BEREIKBAARHEID</h5>
                        <p>Parkeren bij de locatie is gratis.
                            <br> Er zijn voldoende parkeerplekken beschikbaar achter de brouwerij. 
                            <br><br> De brouwerij is gelegen op het Zwitsal terrein. 
                            De ingang van dit terrein direct bij de brouwerij is afgesloten.
                            U moet daarom gebruik maken van <strong>ingang Zuid</strong> (zie onderstaande kaart).
                        </p>
                    </div>
                </div>
            </div>
            <!--  // end .row -->
        </div>
    </div>
    <!-- //  end .highlight -->

    <img src="images/zwitsal.png" class="map-zwitsal" alt="plattegrond" />

    <div class="container" id="contact">
        <div class="section-title">
            <h4>AANMELDEN</h4>
            <p>Vul onderstaand formulier in om u aan te melden voor het afscheid.
            Het is <strong>niet</strong> de bedoeling dat u iets meeneemt voor Maria, maar het is de bedoeling dat u na afloop wat meeneemt naar huis: het inzicht in het wettelijke recht van een kind om kind te zijn.</p>
        </div>

        <div class="contact-form bottom-space-xl wow fadeInUp">
            <div class="row">
                <div class="col-md-6 col-md-offset-3">
                    <SignupForm />
                </div>
            </div>
        </div>

        <div class="section-title">
            <p>Voor vragen of meer informatie kunt u zich wenden tot Saskia Blom, <a href="mailto:s.blom@cjgapeldoorn.nl">s.blom@cjgapeldoorn.nl</a>,  
            <a href="tel:+31555805359">055 580 53 59</a></p>
        </div>
    </div>
    <!-- // end .container -->

    <footer>
        <p> <small class="text-muted">Copyright © 2019. All rights reserved. Made in Amsterdam.</small></p>

    </footer>

    <a href="#top" class="back_to_top"><img src="images/back_to_top.png" alt="back to top"></a>

  </div>
</template>

<script>
import SignupForm from './components/SignupForm';

export default {
  name: 'App',

  components: {
      SignupForm
  }
}
</script>

<style>

</style>
