<template>
  <div class="header">

    <!--    <TopName></TopName>-->

    <!--    <div class="nav">-->
    <!--      <img alt="navigation menu button" src="../assets/burger.svg">-->
    <!--    </div>-->

    <HeaderImage></HeaderImage>
    <!--    <HeaderContent></HeaderContent>-->

  </div>
</template>

<script>
// import TopName from '@/components/TopName.vue'
import HeaderImage from '@/components/HeaderImage.vue'
// import HeaderContent from '@/components/HeaderContent.vue'

export default {
  name: 'Header',
  components: {
    // TopName,
    HeaderImage,
    // HeaderContent,
  },
  props: {
    msg: String
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.header {
  overflow: hidden;
  background-image: linear-gradient(#062041, #020B17);
  width: 100vw;
  height: 100vh;
}

</style>
