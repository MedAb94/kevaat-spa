<template>
  <div>
    <slider />
    <!-- ======= About Section ======= -->
    <section id="about" class="about">
      <div class="container">
        <div class="row justify-content-between">
          <div
            class="col-lg-5 d-flex align-items-center justify-content-center about-img"
          >
            <img
              src="/about.jpg"
              class="img-fluid rounded"
              alt="Kevaat"
              data-aos="zoom-in"
            />
          </div>
          <div class="col-lg-6 pt-5 pt-lg-0 ">
            <h3 data-aos="fade-up" class="w-full-md text-center">
              PRESENTATION
            </h3>
            <p data-aos="fade-up" data-aos-delay="0" class="text-justify">
              L'Institut “Kevaat Training” a pour mission centrale d'initier,
              développer et renforcer les compétences spécialisées au sein des
              entreprises et des administrations. Il met à votre disposition des
              programmes, des séminaires et des cycles de formation, assistés
              par informatique, spécialement conçus pour répondre aux besoins
              évolutifs du marché du travail. L'Institut Kevaat Training vous
              permet ainsi de parfaire la maitrise du savoir-faire, acquérir les
              nouvelles techniques de qualité, d'organisation et d'efficience en
              vue d'améliorer votre compétitivité.
            </p>
            <p data-aos="fade-up">
              <a href="assets/brochure.pdf" target="_blank">
                <button class="btn btn-primary">Voir brochure</button>
              </a>
              <a href="assets/brochure.pdf" target="_blank">
                <button class="btn btn-primary">Voir co-working</button>
              </a>
            </p>
            <div class="row">
              <div class="col-md-6" data-aos="fade-up" data-aos-delay="100">
                <i class="bx bx-receipt"></i>
                <h4>Gestion de la qualité, hygiène et sécurité</h4>
                <p class="text-justify">
                  Nous proposons plusieurs formation dans le domaine de la
                  gestion de qualité, hygiène et sécurité et ses branches.
                </p>
              </div>
              <div class="col-md-6" data-aos="fade-up" data-aos-delay="200">
                <i class="bx bx-dollar-circle"></i>
                <h4>Banques et finances</h4>
                <p class="text-justify">
                  <strong>KEVAAT </strong>est un pionnier dans le domaine de la
                  formation financière, il agit rapidement et de manière rapide
                  et coopère avec d‘autres organisations dans le domaine.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- End About Section -->

    <!-- ======= actualites Section ======= -->
    <section>
      <v-container>
        <div class="section-title" data-aos="fade-up">
          <h2>Actualités</h2>
          <p>Les nouvelles formations et actualités de l'institut</p>
        </div>

        <v-row>
          <v-col cols="12" md="6" sm="12" v-for="i in 4" :key="i">
            <v-container>
              <v-card class="mx-auto" max-width="100%" outlined>
                <v-list-item three-line>
                  <v-list-item-content>
                    <v-list-item-title class="headline mb-1">
                      Headline 5
                    </v-list-item-title>
                    <v-list-item-subtitle>
                      Greyhound divisely hello coldly fonwderfully Lorem ipsum
                      dolor sit amet consectetur adipisicing elit. Officiis
                      consequuntur tenetur, deserunt delectus aut assumenda!
                      Delectus quos dolore, nesciunt saepe eos asperiores soluta
                      magnam sint nulla quo. Cupiditate, quibusdam optio!
                    </v-list-item-subtitle>
                  </v-list-item-content>

                  <v-list-item-avatar
                    tile
                    size="80"
                    color="grey"
                  ></v-list-item-avatar>
                </v-list-item>

                <v-card-actions class="text-center">
                  <v-btn text href="actualites/test">
                    EN SAVOIR PLUS
                  </v-btn>
                </v-card-actions>
              </v-card>
            </v-container>
          </v-col>
          <div class="ml-auto">
            <a href="/info"> Voir tous les actualités</a>
          </div>
        </v-row>
      </v-container>
    </section>
    <!-- End actualites Section -->

    <!-- ======= Clients Section ======= -->
    <section id="References" class="clients ">
      <div class="container">
        <div class="section-title" data-aos="fade-up">
          <h2>Ils nous ont fait confiance</h2>
        </div>
      </div>
      <div class="container-fluid py-3">
        <v-slide-group show-arrows>
          <v-slide-item v-for="item in images" :key="item" class="mx-4">
            <v-img :src="item" contain max-width="250px" max-height="200px">
            </v-img>
          </v-slide-item>
        </v-slide-group>
      </div>
    </section>
    <!-- End Clients Section -->
  </div>
</template>

<script>
import Slider from "../components/Slider";
export default {
  components: { Slider },
  data() {
    return {
      images: [
        "/clients/1.png",
        "/clients/2.png",
        "/clients/3.png",
        "/clients/4.png",
        "/clients/5.png",
        "/clients/6.png",
        "/clients/7.png",
        "/clients/8.png",
        "/clients/12.png",
        "/clients/9.png",
        "/clients/10.png",
        "/clients/11.png",
        "/clients/13.png",
        "/clients/14.png"
      ]
    };
  },
  head: {
    title: "Accueil"
  }
};
</script>
<style scoped>
/*--------------------------------------------------------------
# Hero Section
--------------------------------------------------------------*/
#hero {
  width: 100%;
  height: 70vh;
  background: #28a745;
  border-bottom: 2px solid #fcebe3;
  margin: 72px 0 -72px 0;
}

#hero h1 {
  margin: 0 0 10px 0;
  font-size: 48px;
  font-weight: 700;
  line-height: 56px;
}

#hero h2 {
  color: #e3e8f4;
  margin-bottom: 50px;
  font-size: 24px;
}

#hero .btn-get-started {
  font-family: "Raleway", sans-serif;
  font-weight: 500;
  font-size: 16px;
  letter-spacing: 1px;
  display: inline-block;
  padding: 8px 28px;
  border-radius: 3px;
  transition: 0.5s;
  margin: 10px;
  color: #fff;
  background: #eb5d1e;
}

#hero .btn-get-started:hover {
  background: #ef7f4d;
}

#hero .animated {
  animation: up-down 2s ease-in-out infinite alternate-reverse both;
}

@media (min-width: 1024px) {
  #hero {
    background-attachment: fixed;
  }
}

@media (max-width: 991px) {
  #hero {
    height: calc(100vh - 72px);
  }
  #hero .animated {
    -webkit-animation: none;
    animation: none;
  }
  #hero .hero-img {
    text-align: center;
  }
  #hero .hero-img img {
    width: 50%;
  }
}

@media (max-width: 768px) {
  #hero h1 {
    font-size: 28px;
    line-height: 36px;
  }
  #hero h2 {
    font-size: 18px;
    line-height: 24px;
    margin-bottom: 30px;
  }
  #hero .hero-img img {
    width: 70%;
  }
}

@media (max-width: 575px) {
  #hero .hero-img img {
    width: 80%;
  }
}

@-webkit-keyframes up-down {
  0% {
    transform: translateY(10px);
  }
  100% {
    transform: translateY(-10px);
  }
}

@keyframes up-down {
  0% {
    transform: translateY(10px);
  }
  100% {
    transform: translateY(-10px);
  }
}

/*--------------------------------------------------------------
# About
--------------------------------------------------------------*/
.about h3 {
  font-weight: 700;
  font-size: 34px;
}

.about h4 {
  font-size: 20px;
  font-weight: 700;
  margin-top: 5px;
}

.about i {
  font-size: 48px;
  margin-top: 15px;
  color: green;
}

.about p {
  font-size: 15px;
  color: #5a6570;
}

@media (max-width: 991px) {
  .about .about-img img {
    max-width: 70%;
  }
}

@media (max-width: 767px) {
  .about .about-img img {
    max-width: 90%;
  }
}
</style>
