<template>
  <v-app>
    <Header />
    <router-view />
    <Footer />
    <img
      src="./assets/whatsapp.png"
      width="40"
      class="whatsapp-fixed mb-3 mr-3"
    />
  </v-app>
</template>

<script>
import Header from "./components/CustomHeader.vue";
import Footer from "./components/CustomFooter.vue";

export default {
  name: "App",
  components: {
    Header,
    Footer,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Lato:wght@100;300;900&display=swap");

* {
  font-family: "Lato", sans-serif;
}

.whatsapp-fixed {
  position: fixed;
  bottom: 0;
  right: 0;
}
</style>
