<template>
  <div class="container">
    <v-breadcrumbs divider=">"></v-breadcrumbs>
    <v-row align="center">
      <v-col cols="12" md="6" sm="12">
        <img
          src="/about.jpg"
          class="img-fluid rounded"
          alt="Kevaat"
          data-aos="zoom-in"
        />
      </v-col>
      <v-col cols="12" md="6" sm="12">
        <h3 class="text-center mt-5">Post title hello kevaat</h3>{{this.$route.params.post}}
        <p class="text-center caption">Publié le: 17/11/2020</p>
      </v-col>
      <v-col cols="12">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit
        saepe repellat aspernatur officiis labore magnam similique excepturi
        maxime error sed obcaecati, omnis, unde magni nobis, mollitia harum
        dicta perferendis inventore! Lorem ipsum dolor sit amet consectetur
        adipisicing elit. Reprehenderit saepe repellat aspernatur officiis
        labore magnam similique excepturi maxime error sed obcaecati, omnis,
        unde magni nobis, mollitia harum dicta perferendis inventore! Lorem
        ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit saepe
        repellat aspernatur officiis labore magnam similique excepturi maxime
        error sed obcaecati, omnis, unde magni nobis, mollitia harum dicta
        perferendis inventore! Lorem ipsum dolor sit amet consectetur
        adipisicing elit. Reprehenderit saepe repellat aspernatur officiis
        labore magnam similique excepturi maxime error sed obcaecati, omnis,
        unde magni nobis, mollitia harum dicta perferendis inventore!
      </v-col>
    </v-row>
  </div>
</template>
