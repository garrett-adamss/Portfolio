<template>
  <header>
    <Navbar />
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
</style>
