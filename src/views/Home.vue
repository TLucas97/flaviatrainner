<template>
  <div class="home">
    <Profile />
    <About />
    <Personal />
  </div>
</template>

<script>
import Profile from "../components/Profile.vue";
import About from "../components/About.vue";
import Personal from "../components/Personal.vue";

export default {
  components: {
    Profile,
    About,
    Personal,
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
</style>
