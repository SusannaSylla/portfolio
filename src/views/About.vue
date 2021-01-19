<template>
  <div class="about">
    <Header/>

    <AboutMainContent/>

    <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import AboutMainContent from '@/components/AboutMainContent'
import Footer from '@/components/Footer.vue'

export default {
  name: 'About',
  components: {
    Header,
    AboutMainContent,
    Footer
  }
}
</script>

<style lang="scss" scoped>
/deep/ .title {
  visibility: hidden;
}

/deep/ .portfolio-title {
  visibility: hidden;
}

/deep/ .face {
  left: 50%;
}

/deep/ .circles {
  left: 51%;
}

/deep/ .footer {
  top: 310vh;
  position: absolute;
}
</style>