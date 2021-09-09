<template>
  <div id="app">
            <header></header>
            <div class="wrapper">
                <!-- Hero-->
                <main class="module-cover">
                  <section>
                      <div class="container">
                          <div class="row">
                              <div class="col-md-8">
                                  <nav aria-label="Breadcrumb" v-animate-onscroll="'animated flip'">
                                    <ul class="breadcrumb">
                                        <li class="m-1"><a href="">école</a></li>
                                        <li class="m-1"><a href="">Robotique</a></li>
                                        <li class="m-1"><span aria-current="page">industrie du futur</span></li>
                                    </ul>
                                  </nav>
                                  <h1 class="title animated tada">Un printemps robotique à Arts et Métiers</h1>
                                  <p>Le campus Arts et Métiers de Lille, se positionne comme un acteur incontournable de la robotique par ses activités de formation, de recherche et de transfert technologique.</p>
                                  <a href="#"><i>> Lire plus</i></a>
                                  
                              </div>
                          </div>
                      </div>
                  </section>
                  <!-- Hero end-->
                  <section class="horizontal-list">
                      <image-three />
                      <VueAnimateOnScroll />
                  </section>
                </main>
                <section>
                      <div class="container">
                          <div class="row">
                              <div class="col-md-8">
                                  <div class="row" data-aos="fade-up"
                                    data-aos-offset="200"
                                    data-aos-delay="50"
                                    data-aos-duration="1000"
                                    data-aos-easing="ease-in-out"
                                    data-aos-mirror="true"
                                    data-aos-once="false"
                                    data-aos-anchor-placement="top-center">
                                      <div class="col-md-3">
                                          <h2 class="mt-5" @click='toggle = !toggle'>école</h2>
                                          <ul class="mb-2" v-show='toggle'>
                                              <li>Présentation</li>
                                              <li>Réseau Arts et Métiers partenaires</li>
                                              <li>Une école engagée</li>
                                              <li>Les campus Arts et Métiers</li>
                                              <li>International</li>
                                              <li>Agenda</li>
                                              <li>Actualités</li>
                                              <li>L’école recrute</li>
                                              <li>Marchés publics</li>
                                          </ul>
                                          <img class="mt-2 mb-5" src="./assets/img/institut-carnot.png" />
                                      </div>
                                      <div class="col-md-3" v-animate-onscroll.repeat="{down: 'animated flip'}">
                                          <h2 class="mt-5">Formation</h2>
                                          <ul class="mb-2">
                                              <li>Bachelor de technologie</li>
                                              <li>Ingénieur généraliste</li>
                                              <li>Ingénieur de spécialité</li>
                                              <li>Masters recherche</li>
                                              <li>Mastères spécialisés et MBA</li>
                                              <li>Doctorat</li>
                                              <li>étudiants internationaux</li>
                                              <li>Formation tout au long de la vie</li>
                                              <li>MOOCS</li>
                                              <li>Vie étudiante</li>
                                          </ul>
                                          <img class="mt-2 mb-5" src="./assets/img/paris-tech.png" />
                                      </div>
                                      <div class="col-md-3">
                                          <h2 class="mt-5">Recherche</h2>
                                          <ul class="mb-2">
                                              <li>Filières de recherche</li>
                                              <li>Les réseaux nationaux de la connaissance (RNC)</li>
                                              <li>Recherche partenariale</li>
                                              <li>Publications</li>
                                          </ul>
                                          <img class="mt-2 mb-5" src="./assets/img/hesam.png" />
                                      </div>
                                      <div class="col-md-3">
                                          <h2 class="mt-5">Entreprise</h2>
                                          <ul class="mb-2">
                                              <li>Recruter nos étudiants</li>
                                              <li>Soutenir l’école</li>
                                              <li>Transfert et valorisation</li>
                                              <li>Entrepreneuriat</li>
                                              <li>Former vos collaborateurs</li>
                                              <li>Organiser un évènement</li>
                                          </ul>
                                      </div>
                                  </div>
                              </div>
                              <div class="col-md-4 map-responsive">
                                 <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2626.3193900091924!2d2.356034915836622!3d48.83304621044489!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47e6718c8bebce9f%3A0x9220c0c18f5aa958!2sArts%20et%20M%C3%A9tiers%20-%20Campus%20de%20Paris%20-%20HESAM%20Universit%C3%A9!5e0!3m2!1sfr!2sfr!4v1630851010235!5m2!1sfr!2sfr" width="100%" height="600" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
                              </div>
                          </div>
                      </div>
                  </section>
                <!-- Footer-->
                <footer>
                            <div class="row">
                                <div class="col-md-5">
                                    <h6>© école Nationale Supérieur des Arts et Métiers 2016</h6>
                                </div>
                                <div class="col-md-1">
                                    <h6><a href="#">Rejoignez-nous</a></h6>
                                </div>
                                <div class="col-md-1">
                                    <h6><a href="#">Contactez-nous</a></h6>
                                </div>
                                <div class="col-md-1">
                                    <h6><a href="#">Plan d'accès</a></h6>
                                </div>
                                <div class="col-md-1">
                                    <h6><a href="#">Mentions légales</a></h6>
                                </div>
                                <div class="col-md-3">
                                    <h6><i>Agence fidesio</i></h6>
                                </div>
                            </div>
                </footer>
                <!-- Footer end-->
            </div>
            <!-- Wrapper end-->
            <!-- To top button--><a class="scroll-top" href="#top"><i class="fas fa-angle-up"></i></a>
    
  </div>
</template>

<script>

import ImageThree from "./components/image-three";
import VueAnimateOnScroll from 'vue-animate-onscroll';
export default {
  name: 'App',
  components: {
    ImageThree,
    VueAnimateOnScroll,
  },
  data(){
    return {
        toggle: true,
      };
  },
  methods: {
  },
  props: []
}
</script>

<style></style>
