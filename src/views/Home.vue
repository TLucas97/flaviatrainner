<template>
  <div class="home pb-12">
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
  components: {
    Profile,
    About,
    Personal,
    Contact,
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

.content {
  width: 95%;
  margin: 0 auto;
}
</style>
