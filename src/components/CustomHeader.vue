<template>
  <div class="header d-flex justify-space-between align-center">
    <div class="d-flex align-center">
      <div class="pr-2">
        <h1>{{ title }}</h1>
      </div>
      <div>
        <img src="../assets/working-heart.png" width="35" />
      </div>
    </div>
    <div>
      <!-- <img v-b-toggle.sidebar-no-header src="../assets/menu.png" width="35" /> -->
      <v-icon v-b-toggle.sidebar-no-header dark right size="40">
        mdi-menu
      </v-icon>
    </div>
    <b-sidebar
      id="sidebar-no-header"
      ref="mySidebar"
      class="index"
      aria-labelledby="sidebar-no-header-title"
      no-header
      shadow
      right
      backdrop
      width="175px"
    >
      <template>
        <div class="p-3 white--text sidebar-bg">
          <h3 id="sidebar-no-header-title" class="font-weight-bold text-center">
            Flavia Silva <br />
            <img src="../assets/working-heart.png" width="35" /> <br />
            <small class="h4-small">Personal Trainer</small>
          </h3>
          <div
            class="d-flex justify-content-center align-center flex-column mt-7"
          >
            <p @click="profileScroll">Início</p>
            <p @click="aboutScroll">Sobre mim</p>
            <p @click="personalScroll">Personal</p>
            <p @click="contactScroll">Contato</p>
          </div>
        </div>
      </template>
    </b-sidebar>
  </div>
</template>

<script>
export default {
  data() {
    return {
      title: "Flavia Silva",
    };
  },
  methods: {
    contactScroll() {
      document.getElementById("contact").scrollIntoView({
        behavior: "smooth",
      });
      this.$refs.mysidebar.hide();
    },
    profileScroll() {
      document.getElementById("profile").scrollIntoView({
        behavior: "smooth",
      });
      this.$refs.mysidebar.hide();
    },
    aboutScroll() {
      document.getElementById("about").scrollIntoView({
        behavior: "smooth",
      });
      this.$refs.mysidebar.hide();
    },
    personalScroll() {
      document.getElementById("personal").scrollIntoView({
        behavior: "smooth",
      });
      this.$refs.mysidebar.hide();
    },
  },
};
</script>

<style scoped>
.header {
  width: 100%;
  position: fixed;
  top: 0;
  padding: 0.8em;
  background: #313552;
  color: #ffffff;
  z-index: 1000;
}

.sidebar-bg {
  background: #313552;
  height: 100%;
}

h1 {
  font-weight: bold;
  padding: 0;
  margin: 0;
}

.h4-small {
  font-size: 0.6em;
}

p {
  margin-bottom: 1.5em !important;
  padding-bottom: 0.2em;
  font-weight: bold;
  border-bottom: 1px solid #e7d2d2;
  letter-spacing: 1.2px;
}
</style>
