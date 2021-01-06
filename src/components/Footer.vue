<template>
  <div class="footer">
    <div class="separation-line"></div>
    <p>Made with vue.js by Susanna Saadi</p>
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

.separation-line {
  background-color: #FFF;
  height: 0.4vh;
  width: 100vw;
}

p {
  color: #FFFFFF;
  font-weight: 500;
  font-family: Montserrat, sans-serif;
  margin: 0 auto;
  position: absolute;
  top: 50%;
}
</style>