<template>
  <div>
    <v-row>
      <v-col cols="12">
        <v-container>
          <v-card
            class="mx-auto my-2"
            max-width="100%"
            outlined
            v-for="i in 3"
            :key="i"
          >
            <v-row>
              <v-col
                cols="12"
                md="10"
                sm="12"
                class="px-8"
                order-md="2"
                order="1"
              >
                <h3>
                <a href="/actualites/test" target="_blank" >Headline 5</a>

                </h3>
                <p>
                  Greyhound divisely hello coldly fonwderfully Lorem ipsum dolor
                  sit amet consectetur adipisicing elit. Officiis consequuntur
                  tenetur, deserunt delectus aut assumenda!
                </p>
              </v-col>
              <v-col
                cols="12"
                md="2"
                sm="12"
                xs="12"
                class="text-center"
                order-md="2"
                order-sm="1"
                order-xs="1"
              >
                <img
                  src="/about.jpg"
                  class="w-100"
                  alt="Kevaat"
                  data-aos="zoom-in"
                />
              </v-col>
            </v-row>
          </v-card>
        </v-container>
      </v-col>
    </v-row>

    <v-sheet class="pa-3">
      <v-skeleton-loader
        class="mx-auto"
        type="card"
      ></v-skeleton-loader>
    </v-sheet>
  </div>
</template>
<script>
export default {};
</script>
