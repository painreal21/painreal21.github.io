<template>
  <div id="app">
    <Navbar />

    <!-- Sections -->
    <section id="home">
      <Home />
    </section>

    <section id="about">
      <About />
    </section>

    <section id="projects">
      <Projects />
    </section>

    <section id="skills">
      <Skills />
    </section>

    <section id="contact">
      <Contact />
    </section>
  </div>
</template>

<script>
import AOS from 'aos'
import 'aos/dist/aos.css'

import Navbar from './components/Navbar.vue'
import Home from './components/Home.vue'
import About from './components/About.vue'
import Projects from './components/Projects.vue'
import Skills from './components/Skills.vue'
import Contact from './components/Contact.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Home,
    About,
    Projects,
    Skills,
    Contact
  },
  mounted() {
    AOS.init({
      duration: 1000,
      once: true,
    });
  }
}
</script>

<style>
body {
  margin: 0;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  background-color: #0f0f0f;
  color: white;
  scroll-behavior: smooth;
}

#app {
  overflow-x: hidden;
  padding-top: 60px; /* Adjust to navbar height */
}
</style>
