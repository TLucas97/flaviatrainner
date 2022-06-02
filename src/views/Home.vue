<template>
  <div class="home pb-12" :class="dark_mode">
    <div class="dark-icon mb-16 mr-3">
      <v-icon size="40" color="black" @click="toggleDarkMode"
        >mdi-brightness-6</v-icon
      >
    </div>
    <Profile id="profile" />
    <div class="content">
      <About id="about" />
      <Personal id="personal" />
    </div>
    <Contact id="contact" />
  </div>
</template>

<script>
import Profile from "../components/Profile.vue";
import About from "../components/About.vue";
import Personal from "../components/Personal.vue";
import Contact from "../components/Contact.vue";

export default {
  data() {
    return {
      dark_mode: "",
    };
  },
  components: {
    Profile,
    About,
    Personal,
    Contact,
  },
  methods: {
    toggleDarkMode() {
      this.dark_mode = this.dark_mode ? "" : "dark-mode";
    },
  },
};
</script>

<style scoped>
.home {
  width: 100%;
  height: 100%;
  background: #f9f3ee;
  padding-top: 5.5em;
}

.dark-mode {
  background: #292929;
  color: #ffffff !important;
}

.dark-mode a {
  color: #ffffff !important;
}

.dark-icon {
  position: fixed;
  bottom: 0;
  right: 0;
}

.content {
  width: 95%;
  margin: 0 auto;
}
</style>
