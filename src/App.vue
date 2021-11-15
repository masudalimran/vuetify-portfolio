<template>
<v-app>
  <Header/>
  <v-main>
    <HeroComponent/>
    <about-us/>
    <portfolio/>
    <project/>
    <gallery/>
    <contact-us/>
    <Footer/>
  </v-main>
</v-app>
</template>

<script>
import AboutUs from './components/AboutUs.vue';
import ContactUs from './components/ContactUs.vue';
import Footer from './components/Footer.vue';
import Gallery from './components/Gallery.vue';
import Header from './components/Header.vue'
import HeroComponent from './components/HeroComponent.vue'
import Portfolio from './components/Portfolio.vue';
import Project from './components/Project.vue';
export default {
  name: 'App',
  components: {
    Header,
    HeroComponent,
    AboutUs,
    Portfolio,
    Project,
    Gallery,
    ContactUs,
    Footer,
  },
};
</script>
