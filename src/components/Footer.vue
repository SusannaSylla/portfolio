<template>
  <div class="footer">
    <div class="separation-line"></div>
    <div class="loveLogo"><p>Made with <span><img src="../assets/loveLogo.svg" alt="love"></span> by Susanna Saadi</p></div>
  </div>
</template>

<script>
export default {
  name: "Footer"
}
</script>

<style scoped>
.footer {
  background-color: #B53D4B;
  height: 11vh;
  width: 100vw;
  display: flex;
  justify-content: center;
  position: relative;
}
img {
  width: 6%;
  height: 6%;
}

.separation-line {
  background-color: #FFF;
  height: 0.4vh;
  width: 100vw;
}

.loveLogo {
  color: #FFFFFF;
  font-weight: 500;
  font-family: Montserrat, sans-serif;
  margin: 0 auto;
  position: absolute;
  top: 40%;
  left: 19%;
}
</style>