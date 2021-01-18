<template>
  <div class="aboutMainContent">
    <AboutSkills></AboutSkills>
    <Certificate></Certificate>




    <button>
            <a href="../assets/SusannaSCV.pdf" target="_blank">Download CV...</a>
    </button>
  </div>
</template>

<script>

import AboutSkills from '@/components/AboutSkills.vue'
import Certificate from '@/components/Certificate.vue';

export default {
  name: "AboutMainContent",
  components: {
    AboutSkills,
    Certificate
  },
}
</script>

<style scoped>
.aboutMainContent {
  background-image: linear-gradient(#020B17, #062041);
  background-repeat: no-repeat;
  height: 200vh;
}
</style>