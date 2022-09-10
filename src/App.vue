<template>
  <header>
    <div class="row align-items-center">
      <h2 class="col-9 title"><b>Portfolio</b></h2>
      <a href="#" class="nav-title tags col-1">About me</a>
      <a href="#" class="nav-title tags col-1">Projects</a>
      <a href="#" class="nav-title tags col-1">Contact</a>
    </div>
  </header>
  <main>
    <!-- <router-view /> -->
    <HomePage />
    <AboutMePage />
    <ContactMePage/>
  </main>
  <footer>
    <div class="row align-items-center justify-content-around p-3">
      <a href="https://www.linkedin.com/in/garrett-adamss/" class="footer-title col-4 text-center">LinkedIn</a>
      <a href="https://github.com/garrett-adamss" class="footer-title col-4 text-center">Github</a>
      <a href="https://www.instagram.com/garrett.adamsss/" class="footer-title col-4 text-center">Instagram</a>
    </div>
  </footer>
</template>

<script>
import { computed } from 'vue';
import { AppState } from './AppState';
import AboutPage from "./pages/AboutPage.vue";
import HomePage from "./pages/HomePage.vue";
import ContactMePage from './pages/ContactMePage.vue';
import AboutMePage from './pages/AboutMePage.vue';

export default {
  name: "App",
  setup() {
    return {
      appState: computed(() => AppState)
    };
  },
  components: { AboutPage, HomePage, ContactMePage, AboutMePage }
}
</script>
<style lang="scss">
@import "./assets/scss/main.scss";
@import 'https://fonts.googleapis.com/css?family=Roboto+Mono:100';

@keyframes slideInFromLeft {
  0% {
    transform: translateX(-100%);
  }

  100% {
    transform: translateX(0);
  }
}

header {
  animation: 1s ease-out 0s 1 slideInFromLeft;
  padding: 30px;
  font-family: 'Roboto Mono', monospace;
  a {
    color: black;
  }
}

main {
  font-family: 'Roboto Mono', monospace
}

footer {
  font-family: 'Roboto Mono', monospace;

  a {
    color: black;
  }
}
</style>
