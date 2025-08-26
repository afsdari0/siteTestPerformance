<template>
  <v-app>
    <Navbar />
    <v-main>
      <Hero />
      <Services />
      <About />
      <Contact />
    </v-main>
    <Footer />
  </v-app>
</template>

<script setup>
import Navbar from './components/Navbar.vue'
import Hero from './components/Hero.vue'
import Services from './components/Services.vue'
import About from './components/About.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'
</script>
<style>
html {
  scroll-behavior: smooth;
}

</style>