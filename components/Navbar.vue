<template>
  <!-- ======= Header ======= -->
  <header id="header">
    <div class="container-fluid d-flex">
      <div class="logo mr-auto">
        <!--            <h1 class="text-light navbar-brand"><a href="index.html">
            <span>KEVAAT Training</span></a></h1>-->
        <!-- Uncomment below if you prefer to use an image logo -->
        <!-- <a href="/"><img src="/navbrand.png" alt="" class="img-fluid"/></a> -->
        <v-carousel
          hide-delimiters
          :show-arrows="false"
          cycle
          max-width="200px"
          height="50px"
          interval="2000"
          vertical
        >
          <v-carousel-item v-for="(item, i) in 2" :key="i">
            <img src="/navbrand.png" alt="" max-width="200px" class="img-fluid"
          /></v-carousel-item>
        </v-carousel>
      </div>

      <nav class="nav-menu d-none d-lg-block">
        <ul>
          <li><router-link to="/" tag="a">Accueil</router-link></li>
          <li><router-link to="/services" tag="a">Services</router-link></li>
          <li><router-link to="/info" tag="a">Actualités</router-link></li>
          <li>
            <router-link to="/formations" tag="a">Formations</router-link>
          </li>
          <li><router-link to="/contact" tag="a">Contact</router-link></li>

          <li>
            <v-overflow-btn
              :items="langs"
              label="FR"
              append-icon="mdi-translate"
              dense
              flat
            >
            </v-overflow-btn>
          </li>

        </ul>
      </nav>
      <!-- .nav-menu -->
    </div>
  </header>
  <!-- End Header -->
</template>
<script>
export default {
  data() {
    return {
      langs: ["FR", "AR", "EN"],

    };
  }
};
</script>
<style scoped>
/*--------------------------------------------------------------
# Header
--------------------------------------------------------------*/
#header {
  height: 72px;
  transition: all 0.5s;
  z-index: 997;
  transition: all 0.5s;
  padding: 15px 0;
  background: #fff;
  box-shadow: 0px 2px 15px rgba(0, 0, 0, 0.1);
}

#header .logo h1 {
  font-size: 30px;
  margin: 0;
  padding: 6px 0;
  line-height: 1;
  font-weight: 400;
  letter-spacing: 2px;
  color: #eb5d1e !important;
}

#header .logo h1 a,
#header .logo h1 a:hover {
  color: #7a6960;
  text-decoration: none;
}

#header .logo img {
  padding: 0;
  margin: 0;
  max-height: 40px;
}

/*#main {*/
/*  margin-top: 72px;*/
/*}*/

/*--------------------------------------------------------------
# Navigation Menu
--------------------------------------------------------------*/
/* Desktop Navigation */
.nav-menu,
.nav-menu * {
  margin: 0;
  padding: 0;
  list-style: none;
}

.nav-menu > ul > li {
  position: relative;
  white-space: nowrap;
  float: left;
}

.nav-menu a {
  display: block;
  position: relative;
  color: #4e4039;
  padding: 10px 15px;
  transition: 0.3s;
  font-size: 15px;
  font-family: "Open Sans", sans-serif;
}

.nav-menu a:hover,
.nav-menu .active > a,
.nav-menu li:hover > a {
  color: #eb5d1e;
  text-decoration: none;
}

.nav-menu .get-started a {
  background: #eb5d1e;
  color: #fff;
  border-radius: 50px;
  margin: 0 15px;
  padding: 10px 25px;
}

.nav-menu .get-started a:hover {
  background: #ee7843;
  color: #fff;
}

.nav-menu .drop-down ul {
  display: block;
  position: absolute;
  left: 0;
  top: calc(100% - 30px);
  z-index: 99;
  opacity: 0;
  visibility: hidden;
  padding: 10px 0;
  background: #fff;
  box-shadow: 0px 0px 30px rgba(127, 137, 161, 0.25);
  transition: ease all 0.3s;
}

.nav-menu .drop-down:hover > ul {
  opacity: 1;
  top: 100%;
  visibility: visible;
}

.nav-menu .drop-down li {
  min-width: 180px;
  position: relative;
}

.nav-menu .drop-down ul a {
  padding: 10px 20px;
  font-size: 14px;
  font-weight: 500;
  text-transform: none;
  color: #3c1300;
}

.nav-menu .drop-down ul a:hover,
.nav-menu .drop-down ul .active > a,
.nav-menu .drop-down ul li:hover > a {
  color: #eb5d1e;
}

.nav-menu .drop-down > a:after {
  content: "\ea99";
  font-family: IcoFont;
  padding-left: 5px;
}

.nav-menu .drop-down .drop-down ul {
  top: 0;
  left: calc(100% - 30px);
}

.nav-menu .drop-down .drop-down:hover > ul {
  opacity: 1;
  top: 0;
  left: 100%;
}

.nav-menu .drop-down .drop-down > a {
  padding-right: 35px;
}

.nav-menu .drop-down .drop-down > a:after {
  content: "\eaa0";
  font-family: IcoFont;
  position: absolute;
  right: 15px;
}

@media (max-width: 1366px) {
  .nav-menu .drop-down .drop-down ul {
    left: -90%;
  }
  .nav-menu .drop-down .drop-down:hover > ul {
    left: -100%;
  }
  .nav-menu .drop-down .drop-down > a:after {
    content: "\ea9d";
  }
}

/* Mobile Navigation */
.mobile-nav {
  position: fixed;
  top: 0;
  bottom: 0;
  z-index: 9999;
  overflow-y: auto;
  left: -260px;
  width: 260px;
  padding-top: 18px;
  background: #4e4039;
  transition: 0.4s;
}

.mobile-nav * {
  margin: 0;
  padding: 0;
  list-style: none;
}

.mobile-nav a {
  display: block;
  position: relative;
  color: #f9d1c0;
  padding: 10px 20px;
  font-weight: 500;
  transition: 0.3s;
}

.mobile-nav a:hover,
.mobile-nav .active > a,
.mobile-nav li:hover > a {
  color: #f39e7a;
  text-decoration: none;
}

.mobile-nav .get-started a {
  background: #eb5d1e;
  color: #fff;
  border-radius: 50px;
  margin: 15px;
  padding: 10px 25px;
}

.mobile-nav .get-started a:hover {
  background: #ee7843;
  color: #fff;
}

.mobile-nav .drop-down > a:after {
  content: "\ea99";
  font-family: IcoFont;
  padding-left: 10px;
  position: absolute;
  right: 15px;
}

.mobile-nav .active.drop-down > a:after {
  content: "\eaa0";
}

.mobile-nav .drop-down > a {
  padding-right: 35px;
}

.mobile-nav .drop-down ul {
  display: none;
  overflow: hidden;
}

.mobile-nav .drop-down li {
  padding-left: 20px;
}

.mobile-nav-toggle {
  position: fixed;
  right: 15px;
  top: 22px;
  z-index: 9998;
  border: 0;
  background: none;
  font-size: 24px;
  transition: all 0.4s;
  outline: none !important;
  line-height: 1;
  cursor: pointer;
  text-align: right;
}

.mobile-nav-toggle i {
  color: #7a6960;
}

.mobile-nav-overly {
  width: 100%;
  height: 100%;
  z-index: 9997;
  top: 0;
  left: 0;
  position: fixed;
  background: rgba(78, 64, 57, 0.9);
  overflow: hidden;
  display: none;
}

.mobile-nav-active {
  overflow: hidden;
}

.mobile-nav-active .mobile-nav {
  left: 0;
}

.mobile-nav-active .mobile-nav-toggle i {
  color: #fff;
}
.nuxt-link-exact-active {
  border-bottom: solid 3px green;
  color: green !important;
}
</style>
