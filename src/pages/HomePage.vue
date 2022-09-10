<template>
  <div class="home flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <h3>Hi, I'm Garrett</h3>
    <h1>Full Stack Developer</h1>
    <div class="text"></div>
    <p>A developer with an eagerness to learn and challenge myself</p>
  </div>
</template>

<script>
export default {
  name: 'Home',
  setup() {
    return {
    }
  }
}
</script>

<style scoped lang="scss">
.home {
  display: grid;
  height: 80vh;
  place-content: center;
  text-align: center;
  user-select: none;
}

// .dud {
//   color: #757575;
// }
</style>
