<template>
  <div class="aboutSkills">
    <p class="my-skills">My skills:</p>
    <div class="imageBackground"><img src="../assets/skillsChart.svg" alt="my skills chart" class="skillsImage"></div>
  </div>
</template>

<script>

export default {
  name: "AboutSkills"
}
</script>

<style scoped>
.my-skills {
  padding: 3vh 0 0 5vw;
  color: #FFFFFF;
  font-family: 'Montserrat', sans-serif;
  font-weight: 600;
  font-size: 3em;

}

.skillsImage {
  position: absolute;
  top: 114vh;
  width: 90%;
  height: 40%;
}

.imageBackground {
  background-color: #1E2D3C;
  width: 100vw;
  height: 48vh;
  margin-top: 2vh;

}
</style>
