<template>
  <div id="app">
    <!-- Navbar at the top -->
    <Navbar />
    
    <!-- Each section takes the full height of the viewport -->
    <section id="home-section">
      <Home />
    </section>
    <section id="about-section">
      <About />
    </section>
    <section id="projects-section">
      <Projects />
    </section>
    <section id="skills-section">
      <Skills />
    </section>
    <section id="contact-section">
      <Contact />
    </section>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Home from './components/Home.vue';
import About from './components/About.vue';
import Projects from './components/Projects.vue';
import Skills from './components/Skills.vue';
import Contact from './components/Contact.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    Home,
    About,
    Projects,
    Skills,
    Contact
  }
}
</script>

<style scoped>
/* Apply full height for each section */
section {
  height: 100vh; /* 100% of viewport height */
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 20px;
}

/* Optional: Add some distinct background colors for each section */
#home-section {
  background-color: #f8f9fa; /* light grey */
}

#about-section {
  background-color: #f8f9fa; /* light grey */
}

#projects-section {
  background-color: #007bff; /* blue */
  color: white;
}

#skills-section {
  background-color: #6c757d; /* grey */
  color: white;
}

#contact-section {
  background-color: #28a745; /* green */
  color: white;
}

/* Smooth scrolling between sections */
html {
  scroll-behavior: smooth;
}

/* Navbar styling */
nav {
  position: fixed;
  top: 0;
  width: 100%;
  background-color: white;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  z-index: 1000;
}

nav ul {
  display: flex;
  justify-content: space-around;
  list-style: none;
  padding: 10px 0;
}

nav a {
  text-decoration: none;
  color: #000;
  font-weight: bold;
  padding: 10px 20px;
}

nav a:hover {
  color: #007bff;
  transition: color 0.3s ease-in-out;
}
</style>
