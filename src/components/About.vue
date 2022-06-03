<template>
  <div class="about pt-3 mt-3">
    <span id="about"></span>
    <div>
      <h1 class="font-weight-bold text-center">Sobre mim</h1>
      <hr />
      <div class="p-3 font-weight-bold text-justify">
        <p>
          Oi, eu sou a Flavia e eu vou falar um pouco sobre a minha experiência
          como Coach e Personal Trainer. Minha experiência começou ainda na
          universidade onde tive a oportunidade de fazer estágios em várias
          áreas, dentre elas, musculação. Isso me permitiu vivenciar as
          necessidades do público dentro das academias desde crianças até
          idosos, logo depois comecei um estágio em Crosstraining, lá eu iniciei
          do zero pois não tinha experiência nenhuma com o esporte porém logo me
          apaixonei por ele, pela metodología diferenciada de treinamento.
        </p>
        <p>
          Resolvi juntar o que eu havia aprendido e levar para minhas aulas
          dentro do salão de musculação ou nos atendimentos em casa. Ou seja, um
          treinamento diferenciado, onde eu trabalho as capacidades do aluno
          como: mobilidade, flexibilidade, equilíbrio, força, resistência,
          cardio e muito mais. Claro que tudo de acordo com o objetivo, idade e
          limitações desse aluno. E eu quero te ajudar a ter mais saúde e
          qualidade de vida através do exercício físico!
        </p>
      </div>
    </div>
    <div class="carousel">
      <v-carousel
        hide-delimiters
        cycle
        :show-arrows="false"
        interval="3000"
        progress
        height="270"
      >
        <v-carousel-item v-for="(item, i) in items" :key="i">
          <img :src="item.src" class="carousel-img" />
        </v-carousel-item>
      </v-carousel>
    </div>
  </div>
</template>

<script>
export default {
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

hr {
  width: 50px;
  height: 5px;
  background-color: #000000 !important;
  margin: 0 auto;
}

@media (min-width: 650px) {
  .carousel{
    width: 70% !important;
  }
}
</style>
