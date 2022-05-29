<template>
  <div class="home">
    <Profile id="profile" />
    <About id="about" />
  </div>
</template>

<script>
import Profile from "../components/Profile.vue";
import About from "../components/About.vue";

export default {
  components: {
    Profile,
    About,
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
