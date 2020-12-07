<template>
  <v-footer dark>
    <div class="container pb-0">
      <div class="row">
        <div
          class="col-md-4 footer-contact"
          data-aos="fade-up"
          data-aos-delay="100"
        >
          <h4>Kevaat Training</h4>
          <div>
            N°80, Cité NASR, Avenue des Bourses, Ksar
            <br />
            Nouakchott,
            Mauritanie <br />

            <strong>Phone:</strong> +222 45 24 36 29<br />
            <strong>Mobile:</strong> 27 33 47 47 - 22 22 34 52<br />
            <strong>Email:</strong> info@kevaat.com<br />
          </div>
        </div>

        <div
          class="col-md-4 footer-links"
          data-aos="fade-up"
          data-aos-delay="200"
        >
          <h4>Liens utiles</h4>
          <ul style="list-style : none">
            <li>
              <i class="bx bx-chevron-right"></i
              ><NuxtLink to="/" >Accueil</NuxtLink>
            </li>
            <li>
              <i class="bx bx-chevron-right"></i>
              <NuxtLink to="/services" tag="a">Services</NuxtLink>
            </li>
            <li>
              <i class="bx bx-chevron-right"></i
              ><NuxtLink to="/info" tag="a">Actualités</NuxtLink>
            </li>
            <li>
              <i class="bx bx-chevron-right"></i>
              <NuxtLink to="/formations" tag="a">Formations</NuxtLink>
            </li>
            <li>
              <i class="bx bx-chevron-right"></i
              ><NuxtLink to="/contact" tag="a">Contact</NuxtLink>
            </li>
          </ul>
        </div>

        <div class="col-md-4 footer-links"
          data-aos="fade-up"
          data-aos-delay="400">
          <h4>Nos comptes sociaux</h4>
          <p>Suivre Kevaat sur les réseaux sociaux</p>
          <div class="social-links mt-3">
            <a href="#" class="facebook"><i class="bx bxl-facebook"></i></a>
            <a href="#" class="google-plus"><i class="bx bxl-skype"></i></a>
            <a href="#" class="linkedin"><i class="bx bxl-linkedin"></i></a>
          </div>
        </div>
      </div>
    </div>
    <div class="container py-0 text-center">
        <v-divider></v-divider>

      <span>&copy; {{ new Date().getFullYear() }}</span> Copyright
      <strong><span>KEVAAT Training</span></strong
      >. Tous droits Reservés
    </div>
  </v-footer>
</template>
