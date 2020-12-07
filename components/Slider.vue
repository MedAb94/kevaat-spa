<template>
  <v-carousel
    cycle

    height="70vh"

  >
    <v-carousel-item
      v-for="(slide, i) in images"
      :key="i"
    >
      <v-sheet
        height="100%"
      >
        <v-row
          class="fill-height"
          align="center"
          justify="center"
        >
             <img
              :src="'/slider/'+slide"
              class="w-100"
              alt="Kevaat"
            />
        </v-row>
      </v-sheet>
    </v-carousel-item>
  </v-carousel>
</template>
<script>
  export default {
    name: "Slider",
    data: () => ({
      model: 0,
      colors: [
        'primary',
        'secondary',
        'yellow darken-2',
        'red',
        'orange',
      ],
      images:[
        '1.jpg',
        '2.jpg',
        '3.jpg',
        '4.jpg',
      ]
    }),
  }
</script>
