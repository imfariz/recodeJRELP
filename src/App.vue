<template>
  <Navbar />
  <Hero />
  <About />
  <Service />
  <Portofolio />
  <Contact />
  <Closing />
</template>

<script>
import Navbar from './components/Navbar.vue';
import Hero from './components/Hero.vue';
import About from './components/About.vue';
import Service from './components/Services.vue';
import Portofolio from './components/Portofolio.vue';
import Contact from './components/Contact.vue';
import Closing from './components/Close.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    Hero,
    About,
    Service,
    Portofolio,
    Contact,
    Closing,
  },
};
</script>

<style>
#app {
  font-family: 'Poppins', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
