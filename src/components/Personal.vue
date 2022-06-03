<template>
  <div class="personal mt-6 pt-6">
    <span id="personal"></span>
    <div class="p-3 d-flex justify-center align-center flex-column">
      <h1 class="font-weight-bold text-center">Personal Training</h1>
      <hr />
      <small class="grey--text font-weight-bold text-center"
        >Quais são os benefícios de um treino personalizado?</small
      >
    </div>
    <div
      class="d-flex justify-center align-center flex-column mt-4 personal-card"
      data-aos="zoom-in"
      data-aos-duration="1500"
    >
      <div>
        <img src="../assets/personal-b1.png" width="100" />
      </div>
      <p class="font-weight-bold text-center">
        Pode aumentar seu conhecimento sobre condicionamento físico em geral
      </p>
    </div>
    <div
      class="d-flex justify-center align-center flex-column mt-4 personal-card"
      data-aos="zoom-in"
      data-aos-duration="1500"
    >
      <div>
        <img src="../assets/personal-b2.png" width="100" />
      </div>
      <p class="font-weight-bold text-center">
        Pode adaptar sua rotina para atender suas necessidades
      </p>
    </div>
    <div
      class="d-flex justify-center align-center flex-column mt-4 personal-card"
      data-aos="zoom-in"
      data-aos-duration="1500"
    >
      <div>
        <img src="../assets/personal-b4.png" width="100" />
      </div>
      <p class="font-weight-bold text-center">
        Pode te ajudar a aperfeiçoar a execução dos exercícios
      </p>
    </div>
    <div
      class="d-flex justify-center align-center flex-column mt-4 personal-card"
      data-aos="zoom-in"
      data-aos-duration="1500"
    >
      <div>
        <img src="../assets/personal-b3.png" width="100" />
      </div>
      <p class="font-weight-bold text-center">
        Pode te ajudar a definir metas e mantê-lo motivado
      </p>
    </div>
    <div class="p-5 d-flex justify-center align-center">
      <a target="_blank" href="https://contate.me/flaviaptrainner">
        <v-btn color="#313552" class="white--text font-weight-bold"
          >tire suas dúvidas comigo</v-btn
        >
      </a>
    </div>
  </div>
</template>

<script>
import AOS from "aos";
import "aos/dist/aos.css";

export default {
  mounted() {
    AOS.init();
  },
};
</script>

<style scoped>
.personal {
  width: 100%;
}

small {
  font-size: 0.9rem;
}

p {
  margin-top: 0.7em;
}
</style>
