<template>
  <v-app>
    <Header />
    <router-view />
    <Footer class="d-none" />
    <a target="_blank" href="https://contate.me/flaviaptrainner">
      <img
        src="./assets/whatsapp.png"
        width="40"
        class="whatsapp-fixed mb-3 mr-3"
      />
    </a>
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

a {
  text-decoration: none !important;
  color: #ffffff !important;
}

*,
*::before,
*::after {
  box-sizing: border-box;
}

* {
  margin: 0;
}

html,
body {
  height: 100%;
}

body {
  line-height: 1.5;
  -webkit-font-smoothing: antialiased;
}

input,
button,
textarea,
select {
  font: inherit;
}

p,
h1,
h2,
h3,
h4,
h5,
h6 {
  overflow-wrap: break-word;
}

#root,
#__next {
  isolation: isolate;
}
</style>
