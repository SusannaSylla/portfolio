<template>
  <div class="header-images">
    <img class="face" alt="face image" src="../assets/face.png">
    <img class="circles" alt="circles image" src="../assets/circles.svg">
  </div>
</template>

<script>
export default {
  name: "HeaderImage"
}
</script>

<style scoped>
.header-images {
  position: relative;
  height: 100vh;
}

.face {
  display: block;
  position: relative;
  top: 35%;
  left: 64%;
  transform: translate(-50%, -50%);
  z-index: 10;
}

.circles {
  display: block;
  position: absolute;
  top: 35%;
  left: 64%;
  transform: translate(-50%, -50%);
  height: 225vw;
  min-height: 750px;
}
</style>