<template>
  <div class="home no-mobile pb-16">
    <Header :contentHeader="true" class="header-position" />
    <v-row id="desktop-aboutme">
      <v-col>
        <div class="p-2">
          <h1 class="font-weight-bold">Sobre mim</h1>
          <hr />
          <div class="font-weight-bold text-justify">
            <p>
              Oi, eu sou a Flavia e eu vou falar um pouco sobre a minha
              experiência como Coach e Personal Trainer. Minha experiência
              começou ainda na universidade onde tive a oportunidade de fazer
              estágios em várias áreas, dentre elas, musculação. Isso me
              permitiu vivenciar as necessidades do público dentro das academias
              desde crianças até idosos, logo depois comecei um estágio em
              Crosstraining, lá eu iniciei do zero pois não tinha experiência
              nenhuma com o esporte porém logo me apaixonei por ele, pela
              metodología diferenciada de treinamento.
            </p>
            <p>
              Resolvi juntar o que eu havia aprendido e levar para minhas aulas
              dentro do salão de musculação ou nos atendimentos em casa. Ou
              seja, um treinamento diferenciado, onde eu trabalho as capacidades
              do aluno como: mobilidade, flexibilidade, equilíbrio, força,
              resistência, cardio e muito mais. Claro que tudo de acordo com o
              objetivo, idade e limitações desse aluno. E eu quero te ajudar a
              ter mais saúde e qualidade de vida através do exercício físico!
            </p>
          </div>
        </div>
      </v-col>
      <v-col>
        <div class="carousel">
          <v-carousel
            hide-delimiters
            cycle
            :show-arrows="false"
            interval="3000"
            progress
          >
            <v-carousel-item v-for="(item, i) in items" :key="i">
              <img :src="item.src" class="carousel-img" />
            </v-carousel-item>
          </v-carousel>
        </div>
      </v-col>
    </v-row>
    <div class="d-flex justify-center align-center pt-16 mt-10">
      <img class="zoom-in-out-box" src="../assets/arrow-down.png" width="50" />
    </div>
    <div id="desktop-personal" class="mt-16 pt-10">
      <div class="p-3 d-flex justify-center align-center flex-column">
        <h1 class="font-weight-bold text-center">Personal Training</h1>
        <hr />
        <p class="grey--text font-weight-bold text-center">
          Quais são os benefícios de um treino personalizado?
        </p>
      </div>
      <v-row>
        <v-col>
          <div
            class="d-flex justify-center align-center flex-column mt-4 personal-card"
            data-aos="zoom-in"
            data-aos-duration="1500"
          >
            <div>
              <img src="../assets/personal-b1.png" width="100" />
            </div>
            <p class="font-weight-bold text-center pt-3">
              Pode aumentar seu conhecimento sobre condicionamento físico em
              geral
            </p>
          </div>
        </v-col>
        <v-col>
          <div
            class="d-flex justify-center align-center flex-column mt-4 personal-card"
            data-aos="zoom-in"
            data-aos-duration="1500"
          >
            <div>
              <img src="../assets/personal-b2.png" width="100" />
            </div>
            <p class="font-weight-bold text-center pt-3">
              Pode adaptar sua rotina para atender suas necessidades
            </p>
          </div>
        </v-col>
      </v-row>
      <v-row>
        <v-col>
          <div
            class="d-flex justify-center align-center flex-column mt-4 personal-card"
            data-aos="zoom-in"
            data-aos-duration="1500"
          >
            <div>
              <img src="../assets/personal-b4.png" width="100" />
            </div>
            <p class="font-weight-bold text-center pt-3">
              Pode te ajudar a aperfeiçoar a execução dos exercícios
            </p>
          </div>
        </v-col>
        <v-col>
          <div
            class="d-flex justify-center align-center flex-column mt-4 personal-card"
            data-aos="zoom-in"
            data-aos-duration="1500"
          >
            <div>
              <img src="../assets/personal-b3.png" width="100" />
            </div>
            <p class="font-weight-bold text-center pt-3">
              Pode te ajudar a definir metas e mantê-lo motivado
            </p>
          </div>
        </v-col>
      </v-row>
      <div class="p-5 d-flex justify-center align-center">
        <a target="_blank" href="https://contate.me/flaviaptrainner">
          <v-btn
            color="#313552"
            class="white--text font-weight-bold btn-font-size"
            >tire suas dúvidas comigo</v-btn
          >
        </a>
      </div>
    </div>
    <div id="desktop-contacts" class="mt-16 pt-10">
      <div class="d-flex justify-center align-center flex-column">
        <h1 class="font-weight-bold">Contato</h1>
        <hr />
      </div>
      <div class="p-3 icons">
        <b-row class="font-weight-bold">
          <b-col class="d-flex justify-center align-center">
            <a target="_blank" href="https://contate.me/flaviaptrainner">
              <v-icon
                data-aos="zoom-in"
                data-aos-duration="1500"
                size="90"
                color="blue"
                >mdi-cellphone-check</v-icon
              >
            </a>
          </b-col>
          <b-col class="d-flex justify-center align-center">
            <a target="_blank" href="mailto:flaviaptrainer@gmail.com">
              <v-icon
                data-aos="zoom-in"
                data-aos-duration="1500"
                size="90"
                color="red"
                >mdi-email</v-icon
              >
            </a>
          </b-col>
        </b-row>
        <b-row class="font-weight-bold">
          <b-col class="d-flex justify-center align-center">
            <a target="_blank" href="https://contate.me/flaviaptrainner">
              <small>(91) 98353-0355</small>
            </a>
          </b-col>
          <b-col class="d-flex justify-center align-center">
            <a target="_blank" href="mailto:flaviaptrainer@gmail.com">
              <small>flaviaptrainer@gmail.com</small>
            </a>
          </b-col>
        </b-row>
      </div>
      <div class="mt-16">
        <h2 class="font-weight-bold text-center">
          Me acompanhe nas redes sociais!
        </h2>
        <div class="icons mt-6">
          <v-row>
            <v-col class="d-flex justify-center align-center">
              <a
                target="_blank"
                href="https://www.instagram.com/coachflaviasilva/"
              >
                <v-icon
                  data-aos="zoom-in"
                  data-aos-duration="1500"
                  size="90"
                  color="pink"
                  >mdi-instagram</v-icon
                >
              </a>
            </v-col>
            <v-col class="d-flex justify-center align-center">
              <a
                target="_blank"
                href="https://www.facebook.com/Consultoria-Online-com-Flavia-Silva-572778416732056"
              >
                <v-icon
                  data-aos="zoom-in"
                  data-aos-duration="1500"
                  size="90"
                  color="blue"
                  >mdi-facebook</v-icon
                >
              </a>
            </v-col>
          </v-row>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import AOS from "aos";
import "aos/dist/aos.css";
import Header from "../components/CustomHeader.vue";

export default {
  components: {
    Header,
  },
  data() {
    return {
      items: [
        {
          src: require("../assets/slide-photo.jpeg"),
        },
        {
          src: require("../assets/slide-photo2.jpeg"),
        },
        {
          src: require("../assets/slide-photo3.jpg"),
        },
      ],
    };
  },
  mounted() {
    AOS.init();
  },
};
</script>

<style scoped>
.carousel {
  width: 90%;
  margin: 0 auto;
  background-color: #000000;
}

.carousel-img {
  width: 100%;
  height: 100%;
}

.personal-card {
  height: 250px;
  width: 100%;
}

p {
  font-size: 1.2rem;
}

.personal-card p {
  font-size: 1.3rem;
  max-width: 500px;
}

.btn-font-size {
  font-size: 1.3rem;
  padding: 1.3em !important;
}

.icons {
  width: 45%;
  margin: 0 auto;
}

small {
  font-size: 1.3rem;
}

.header-position {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 2000;
}
</style>
