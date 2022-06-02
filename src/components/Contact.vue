<template>
  <div class="contact pb-5">
    <div class="d-flex justify-center align-center flex-column">
      <h1 class="font-weight-bold">Contato</h1>
      <hr />
    </div>
    <div class="p-3">
      <b-row class="font-weight-bold">
        <b-col class="d-flex justify-center align-center">
          <a target="_blank" href="https://contate.me/flaviaptrainner">
            <v-icon size="40" color="blue">mdi-cellphone-check</v-icon>
          </a>
        </b-col>
        <b-col class="d-flex justify-center align-center">
          <a target="_blank" href="mailto:flaviaptrainer@gmail.com">
            <v-icon size="40" color="red">mdi-email</v-icon>
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
      <h5 class="font-weight-bold text-center">
        Me acompanhe nas redes sociais!
      </h5>
      <div class="icons mt-6">
        <v-row>
          <v-col class="d-flex justify-center align-center">
            <a
              target="_blank"
              href="https://www.instagram.com/coachflaviasilva/"
            >
              <v-icon size="60" color="pink">mdi-instagram</v-icon>
            </a>
          </v-col>
          <v-col class="d-flex justify-center align-center">
            <a
              target="_blank"
              href="https://www.facebook.com/Consultoria-Online-com-Flavia-Silva-572778416732056"
            >
              <v-icon size="60" color="blue">mdi-facebook</v-icon>
            </a>
          </v-col>
        </v-row>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.contact {
  width: 100%;
  padding-top: 5.5em;
}

.btn-theme {
  background: #313552;
  color: #ffffff;
  font-weight: bold;
}

.icons {
  max-width: 40%;
  margin: 0 auto;
}
</style>
