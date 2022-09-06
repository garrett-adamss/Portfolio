<template>
  <div class="home flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <button class="btn text-success lighten-30 selectable text-uppercase">
    <a href="#about" ></a>
  </button>
  </div>
</template>

<script>
export default {
  name: 'Home'
}
</script>

<style scoped lang="scss">
.home{
  display: grid;
  height: 110vh;
  place-content: center;
  text-align: center;
  user-select: none;
  .home-card{
    width: 50vw;
    > img{
      height: 200px;
      max-width: 200px;
      width: 100%;
      object-fit: contain;
      object-position: center;
    }
  }
}
</style>
