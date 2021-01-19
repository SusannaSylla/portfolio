<template>
  <div class="aboutMainContent">
    <AboutSkills></AboutSkills>
    <Certificate></Certificate>
    <button class="downloadButton">
      <a href="./SusannaSCV.pdf" target="_blank">Download CV...</a>
    </button>
    <CodeAndContact></CodeAndContact>


  </div>
</template>

<script>

import AboutSkills from '@/components/AboutSkills.vue'
import Certificate from '@/components/Certificate.vue';
import CodeAndContact from '@/components/CodeAndContact.vue';


export default {
  name: "AboutMainContent",
  components: {
    CodeAndContact,
    AboutSkills,
    Certificate
  },
}
</script>

<style scoped>
.aboutMainContent {
  background-image: linear-gradient(#020B17, #062041);
  background-repeat: no-repeat;
  height: 212vh;
  margin-top: -2%;
}

.downloadButton {
  top: 234vh;
  left: 50vw;
  position: absolute;
  transform: translate(-50%, -50%);
  background: #C05A5A;
  border-radius: 45px;
  width: 90%;
  height: 9%;
  border: none;
}

.downloadButton a {
  text-decoration: none;
  color: #FFFFFF;
  font-family: 'Montserrat', sans-serif;
  font-size: 2.3em;
  font-weight: 600;
}

a:link, a:visited {
  color: #FFFFFF;
}

a:hover, a:active {
  color: #1E2D3C;
}

</style>