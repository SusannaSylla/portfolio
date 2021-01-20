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

@media only screen and (min-width: 768px) {

  /deep/ .header {
    .header-images {
      .face {
        top: 50%;
        left: 75%;
        width: 55vh;
        height: 55vh;
      }

      .circles {
        top: 50%;
        left: 75%;
        height: 150vh;
      }
    }

    .header-content {
      .title {
        font-size: 4vw;
        max-width: 50%;
      }

      .portfolio-title {
        font-size: 7vw;
        position: absolute;
        left: 13%;
      }
    }
  }

  /deep/ .content {
    .contentBlock {
      display: flex;

      .picture {
        height: 30em;
        width: 46em;
        margin: 6em;
        background-size: 100%;
      }

      .description {
        font-size: 1.5em;
        padding: 2em;
      }
    }

    .contentBlock:nth-child(odd) {

    }

    .contentBlock:nth-child(even) {

    }
  }


  /deep/ .footer {
    top: unset;
    position: relative;

    .love-logo {
      left: unset;

      p {
        font-size: 1.5em;
        text-align: center;
      }
    }
  }

}

</style>