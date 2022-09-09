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
    <HomePage/>
    <AboutPage/>
  </main>
  <footer>
    <div class="bg-dark text-light text-center p-4">
      Made with 💖 by CodeWorks
    </div>
  </footer>
</template>

<script>
import { computed } from 'vue';
import { AppState } from './AppState';
import AboutPage from "./pages/AboutPage.vue";
import HomePage from "./pages/HomePage.vue";

export default {
    name: "App",
    setup() {
        return {
            appState: computed(() => AppState)
        };
    },
    components: { AboutPage, HomePage }
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
  font-family: 'Roboto Mono', monospace
}
.nav-title{
  color: black;
}
</style>
