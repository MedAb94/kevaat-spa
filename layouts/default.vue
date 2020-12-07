<template>
  <v-app>
    <navbar></navbar>
    <v-main>

        <nuxt />

    </v-main>
      <footer-compo></footer-compo>

  </v-app>

</template>

<script>
import Navbar from "../components/Navbar";
import FooterCompo from "../components/Footer";
export default {
  components: {
    Navbar,
    FooterCompo
  },
  data() {
    return {
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: "Vuetify.js"
    };
  }
};
</script>
<style  >

/*--------------------------------------------------------------
# Sections General
--------------------------------------------------------------*/





.section-title {
  text-align: center;
  padding-bottom: 30px;
}

.section-title h2 {
  font-size: 24px;
  font-weight: 700;
  padding-bottom: 0;
  line-height: 1px;
  margin-bottom: 15px;
}

.section-title p {
  padding-bottom: 15px;
  margin-bottom: 15px;
  position: relative;
  /*font-size: 32px;*/
  font-weight: 700;
  color: #4e4039;
}

.section-title p::after {
  content: '';
  position: absolute;
  display: block;
  width: 60px;
  height: 2px;
  background: green;
  bottom: 0;
  left: calc(50% - 30px);
}
 /* custom scroll bar */
    ::-webkit-scrollbar {
        width: 8px;
        border-radius: 10px 0;
    }

    ::-webkit-scrollbar-track {
        background: transparent;
    }

    ::-webkit-scrollbar-thumb {
        background: green;
        border-radius: 10px 10px 0 0;
    }

    ::-webkit-scrollbar-thumb:hover {
        background: #eb5d1e;
    }
</style>
