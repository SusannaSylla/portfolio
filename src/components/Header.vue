<template>
  <div class="header">

    <HeaderImage></HeaderImage>

    <div class="nav">
      <img alt="navigation menu button" src="../assets/burger.svg">
    </div>

    <TopName></TopName>
    <HeaderContent></HeaderContent>

  </div>
</template>

<script>
import TopName from '@/components/TopName.vue'
import HeaderImage from '@/components/HeaderImage.vue'
import HeaderContent from '@/components/HeaderContent.vue'

export default {
  name: 'Header',
  components: {
    TopName,
    HeaderImage,
    HeaderContent,
  },
  props: {
    msg: String
  },
}
</script>


<style scoped lang="scss">
.header {
  overflow: hidden;
  background-image: linear-gradient(#062041, #020B17);
  width: 100vw;
  height: 100vh;
}

.nav {
  position: absolute;
  right: 0;
  margin: 1em;
  top: 0;
  width: 3em;
}
</style>
