<template>
  <div class="header">

    <HeaderImage></HeaderImage>
    <Introduction></Introduction>
    <Nav></Nav>

    <TopName></TopName>
    <HeaderContent ></HeaderContent>

  </div>
</template>

<script>
import TopName from '@/components/TopName.vue'
import HeaderImage from '@/components/HeaderImage.vue'
import HeaderContent from '@/components/HeaderContent.vue'
import Introduction from "@/components/Introduction"
import Nav from "@/components/Nav";

export default {
  name: 'Header',
  components: {
    Nav,
    TopName,
    HeaderImage,
    HeaderContent,
    Introduction,
  },
  props: {
    msg: String,
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

</style>
