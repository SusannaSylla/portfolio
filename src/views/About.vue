<template>
  <div class="home">
    <Header hideContent/>
    <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'About',
  components: {
    Header,
    Footer
  }
}
</script>

<style lang="scss" scoped>
/deep/ .title {
  visibility: hidden;
}

</style>