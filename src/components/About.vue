<template>
  <div class="about pt-3 mt-3">
    <div>
      <h1 class="font-weight-bold text-center">Sobre mim</h1>
      <hr />
      <div class="p-3 font-weight-bold text-justify">
        <p>
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eius,
          necessitatibus possimus! Hic officiis libero doloribus accusamus
          voluptatum iure provident! Odio expedita illo incidunt est. Quasi
          sapiente voluptatum error dolore. Voluptatem!
        </p>
        <p>
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eius,
          necessitatibus possimus! Hic officiis libero doloribus accusamus
          voluptatum iure provident! Odio expedita illo incidunt est. Quasi
          sapiente voluptatum error dolore. Voluptatem!
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
        height="250"
      >
        <v-carousel-item
          v-for="(item, i) in items"
          :key="i"
          :src="item.src"
        ></v-carousel-item>
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
          src: "https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg",
        },
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/sky.jpg",
        },
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/bird.jpg",
        },
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/planet.jpg",
        },
      ],
    };
  },
};
</script>
''

<style scoped>
hr {
  width: 50px;
  height: 5px;
  background-color: #000000 !important;
  margin: 0 auto;
}

.carousel {
  width: 90%;
  margin: 0 auto;
  background-color: #000000;
}
</style>
