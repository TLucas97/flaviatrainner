<template>
  <v-app id="profile" class="bg-wrapper">
    <Header />
    <vue-page-transition name="fade">
      <router-view />
    </vue-page-transition>
    <Footer />
    <a target="_blank" href="https://contate.me/flaviaptrainner">
      <img
        src="./assets/whatsapp.png"
        width="40"
        class="whatsapp-fixed mb-3 mr-3 heartbeat"
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

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Lato:wght@100;300;900&display=swap");

.bg-wrapper {
  background: #f9f3ee;
}

* {
  font-family: "Lato", sans-serif;
}

@media (max-width: 980px) {
  .no-mobile {
    display: none !important;
  }
}

.whatsapp-fixed {
  position: fixed;
  bottom: 0;
  right: 0;
}

.personal-card {
  width: 75%;
  margin: 0 auto;
  background-color: #31355238;
  color: #000000d3;
  padding: 0.9em;
  border-radius: 0.5em;
}

.home {
  width: 100%;
  height: 100%;
  padding-top: 5.5em;
  /* transition: background 0.5s; */
  transition: all 0.5s;
}

@media (min-width: 980px) {
  .home {
    width: 70%;
    margin: 0 auto;
  }

  .whatsapp-fixed {
    width: 60px;
  }
}

.dark-mode {
  background: #292929 !important;
  color: #ffffff !important;
}

.dark-mode a,
.dark-mode p {
  color: #ffffff !important;
}

a {
  text-decoration: none !important;
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

.v-window {
  &-x-transition,
  &-x-reverse-transition,
  &-y-transition,
  &-y-reverse-transition {
    &-enter-active,
    &-leave-active {
      transition: 1.1s cubic-bezier(0.25, 0.8, 0.5, 1) !important;
    }
  }
}

hr {
  width: 50px;
  height: 5px;
  background-color: #000000 !important;
  margin: 0 auto;
}

@media (min-width: 980px) {
  .hiding {
    display: none !important;
  }
}

.heartbeat {
  -webkit-animation: heartbeat 1.5s ease-in-out infinite both;
  animation: heartbeat 1.5s ease-in-out infinite both;
}

@-webkit-keyframes heartbeat {
  from {
    -webkit-transform: scale(1);
    transform: scale(1);
    -webkit-transform-origin: center center;
    transform-origin: center center;
    -webkit-animation-timing-function: ease-out;
    animation-timing-function: ease-out;
  }
  10% {
    -webkit-transform: scale(0.91);
    transform: scale(0.91);
    -webkit-animation-timing-function: ease-in;
    animation-timing-function: ease-in;
  }
  17% {
    -webkit-transform: scale(0.98);
    transform: scale(0.98);
    -webkit-animation-timing-function: ease-out;
    animation-timing-function: ease-out;
  }
  33% {
    -webkit-transform: scale(0.87);
    transform: scale(0.87);
    -webkit-animation-timing-function: ease-in;
    animation-timing-function: ease-in;
  }
  45% {
    -webkit-transform: scale(1);
    transform: scale(1);
    -webkit-animation-timing-function: ease-out;
    animation-timing-function: ease-out;
  }
}
@keyframes heartbeat {
  from {
    -webkit-transform: scale(1);
    transform: scale(1);
    -webkit-transform-origin: center center;
    transform-origin: center center;
    -webkit-animation-timing-function: ease-out;
    animation-timing-function: ease-out;
  }
  10% {
    -webkit-transform: scale(0.91);
    transform: scale(0.91);
    -webkit-animation-timing-function: ease-in;
    animation-timing-function: ease-in;
  }
  17% {
    -webkit-transform: scale(0.98);
    transform: scale(0.98);
    -webkit-animation-timing-function: ease-out;
    animation-timing-function: ease-out;
  }
  33% {
    -webkit-transform: scale(0.87);
    transform: scale(0.87);
    -webkit-animation-timing-function: ease-in;
    animation-timing-function: ease-in;
  }
  45% {
    -webkit-transform: scale(1);
    transform: scale(1);
    -webkit-animation-timing-function: ease-out;
    animation-timing-function: ease-out;
  }
}
</style>
