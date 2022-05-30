<template>
  <div class="contact">
    <div class="d-flex justify-center align-center flex-column">
      <h1 class="font-weight-bold">Contato</h1>
      <hr />
    </div>
    <div class="p-3">
      <form class="font-weight-bold">
        <div class="form-group mb-2">
          <label for="name">Nome</label>
          <input type="text" class="form-control" id="name" />
        </div>
        <div class="form-group mb-2">
          <label for="email">Email</label>
          <input type="email" class="form-control" id="email" />
        </div>
        <div class="form-group">
          <label for="message">Mensagem</label>
          <textarea class="form-control" id="message" rows="3"></textarea>
        </div>
        <button type="submit" class="btn btn-theme mt-2">Enviar</button>
      </form>
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
  background: #f9f3ee;
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
