<template>
  <v-container id="contact" class="py-16 bg-primary text-white">
    <h2 class="text-h4 font-weight-bold text-center mb-8">Fale Conosco</h2>
    <v-row justify="center">
      <v-col cols="12" md="6">
        <v-form>
          <v-text-field label="Seu Nome" outlined color="white" />
          <v-text-field label="Seu Email" outlined color="white" />
          <v-textarea label="Sua Mensagem" outlined rows="4" color="white" />
          <v-btn block color="secondary" size="large">Enviar</v-btn>
        </v-form>
        <v-container class=" containerCustom1">
            <v-container class=" containerCustom1 mt-4 mb-3">
                <SocialIcons />
            </v-container>
            <v-container class=" containerCustom1 contactInfo d-flex flex-column align-center">
                <h6 class="mb-1">contato@prhima.com.br</h6>
                <h6>(21)99325-2935</h6>
            </v-container>
        </v-container>
      </v-col>
    </v-row>
  </v-container>
</template>
<script setup>
import SocialIcons from "../assets/SocialIcons.vue";

</script>
<style scoped>

#contact {
    height: 86vh !important;
}

.containerCustom1{
    padding: 0 !important;

}

.contactInfo h6 {
    font-size: medium;
}
</style>