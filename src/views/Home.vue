<template>
  <div class="home">
    <Header/>
    <MainContent/>
    <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import MainContent from '@/components/MainContent.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'Home',
  components: {
    Header,
    MainContent,
    Footer
  }
}
</script>
<style lang="scss" scoped>

/deep/ .introduction {
  visibility: hidden;
}

/deep/ #home-link {
  display: none;
}

</style>