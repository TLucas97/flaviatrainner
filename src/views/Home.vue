<template>
  <div class="home pb-12" :class="dark_mode">
    <div class="dark-icon mb-16 mr-3">
      <v-icon size="40" color="black" @click="toggleDarkMode"
        >mdi-brightness-6</v-icon
      >
    </div>
    <div class="hiding">
      <Profile id="profile" />
      <div class="content">
        <About id="about" />
        <Personal id="personal" />
      </div>
      <Contact id="contact" />
    </div>
    <div class="no-mobile">
      <v-row>
        <v-col class="personal-text d-flex justify-start align-center">
          <div class="p-1">
            <h2 class="pb-2 font-weight-bold">
              Que tal garantir uma vida saudável e ativa?
            </h2>
            <h6>
              • Experimente planos de treino que se unem ao seu estilo de vida
            </h6>
            <h6>
              • Foco com alinhamento ao resultado e acompanhamento semanal
            </h6>
            <h6>• Treinos personalizados de fortalecimento e cardio</h6>
            <h6>• Avaliação física e acompanhamento com nutricionista</h6>
            <v-btn
              elevation="8"
              color="success"
              x-large
              dark
              class="mt-5 font-weight-bold btn-increase"
              to="/content"
            >
              SAIBA MAIS
            </v-btn>
          </div>
        </v-col>
        <v-col class="personal-bg"></v-col>
      </v-row>
    </div>
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
.dark-icon {
  position: fixed;
  bottom: 0;
  right: 0;
  z-index: 999;
}

.content {
  width: 95%;
  margin: 0 auto;
}

.personal-bg {
  background: url("../assets/profilepic.png") no-repeat center;
  background-size: cover;
  width: 100%;
  height: 400px;
  border-radius: 0.5em;
}

.personal-text {
  width: 100%;
  height: 400px;
}

h6 {
  font-weight: 600;
  color: #000000b0;
}

@media (min-width: 980px) {
  .dark-icon{
    display: none !important;
  }
}


@media (min-width: 1250px) {
  .personal-bg {
    height: 700px;
  }
}

@media (min-width: 1400px) {
  .personal-text {
    height: 700px;
  }

  .btn-increase {
    font-size: 1.8rem;
    padding: 1em !important;
  }

  h2 {
    font-size: 3rem;
  }

  h6 {
    font-size: 1.5rem;
    margin-bottom: 0.7em;
  }
}
</style>
