<script>
import Hero from "./components/Hero.vue"
import Footer from "./components/Footer.vue"
import Navbar from "./components/Navbar.vue"
import Techniques from "./components/Techniques.vue";
import Projects from "./components/Projects.vue";

export default {
  methods: {
    handleScroll () {
      if (document.body.scrollTop > 100 || document.documentElement.scrollTop > 300) {
            document.getElementById("navbar").style.top = "0";
        } else {
            document.getElementById("navbar").style.top = "-100px";
        }
    }
  },
  beforeMount () {
    window.addEventListener('scroll', this.handleScroll)
  },
  beforeDestroy () {
    window.removeEventListener('scroll', this.handleScroll)
  }
}
</script>

<template>
  <div class="dot-mask">
    <!-- <NuxtRouteAnnouncer />
    <NuxtWelcome /> -->
  </div>
  <header>
    <Navbar />
  </header>
  <div class="content">
    <main>
      <Hero />
      <Techniques />
      <Projects />
    </main>
    <footer>
      <Footer />
    </footer>
  </div>
</template>

<style lang="css">
@import url('https://fonts.googleapis.com/css2?family=Inter:ital,opsz,wght@0,14..32,100..900;1,14..32,100..900&family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');
body {
  color: #464646FF;
  margin:0;
  font-family: "Inter", serif;
  font-optical-sizing: auto;
  font-style: normal;
  scroll-behavior: smooth;
}
.content {
  display: flex;
  flex-direction: column;
  gap:80px;
}
h1{
  margin:0;
}
.dot-mask {
  z-index: -10;
  position: absolute;
  inset: 0;
  height: 100%;
  width: 100%;
  background-image: radial-gradient(#e5e7eb 1px, transparent 1px);
  background-size: 16px 16px;
  -webkit-mask-image: radial-gradient(
    ellipse 50% 50% at 50% 50%,
    #000 60%,
    transparent 100%
  );
  mask-image: radial-gradient(
    ellipse 70% 70% at 50% 50%,
    #000 50%,
    transparent 100%
  );
}
main {
  max-width: 1280px;
  display:flex;
  flex-direction: column;
  justify-content: center;
  margin:0 auto;
  align-items: center;
  gap:80px;
  padding: 0 10px 0 10px;
  transition:all 0.3s ease-in-out;
}
@media only screen and (max-width: 800px) {
  .techniques-container {
    grid-template-columns: repeat(3, 1fr);
  }
}
@media only screen and (max-width: 600px) {
  .techniques-container {
    grid-template-columns: repeat(2, 1fr);
  }
  .projects-container {
    grid-template-columns: repeat(2, 1fr);
  }
}
@media only screen and (max-width: 300px) {
  .techniques-container {
    grid-template-columns: repeat(1, 1fr);
  }
  .projects-container {
    grid-template-columns: repeat(1, 1fr);
  }
}
</style>
