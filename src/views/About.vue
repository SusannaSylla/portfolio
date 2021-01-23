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

/deep/ #about-link {
  display: none;
}

/deep/ .circles {
  filter: hue-rotate(36deg);
}

@media only screen and (min-width: 768px) {

  /deep/ .header {
    .header-images {
      .face {
        top: 50%;
        left: 50%;
        width: 55vh;
        height: 55vh;
      }

      .circles {
        top: 50%;
        left: 50%;
        height: 150vh;
      }
    }

    .introduction {
      top: 75%;
      font-size: 4vh;
      width: 50%;
      min-width: 15em;
      left: 50%;
      transform: translate(-50%, 0);
    }
  }

  /deep/ .aboutMainContent {
    height: initial;

    .imageBackground {
      height: 50vh;
    }

    .my-skills {
      padding: 4vh 0 0 5vw;
    }

    .certificate {
      height: 47vw;

      .lightbox {
        width: 40%;
        position: absolute;
        left: 50%;
        transform: translate(-50%, 0);
      }

      .certificateHeader {
        font-size: 3em;
        padding: 3% 2% 5% 2%;
      }

      .info {
        position: absolute;
        font-size: 1.6em;
        left: 50%;
        margin: -2em 0 0;
        transform: translate(-50%, 0);
      }
    }

    .downloadButton {
      top: unset;
      left: 50%;
      position: relative;
      transform: translate(-50%, 0);
      width: 90%;
      height: 7em;
      margin: 5em 0 10em;

      a {
        font-size: 3em;
      }
    }

    .codeNContact {
      position: relative;

      .code {
        top: unset;
        width: 100vw;
        height: 33em;
        position: unset;

        p {
          padding-top: 2em;
          font-size: 3em;
        }

        a img { // github logo
          position: absolute;
          left: 50%;
          top: 20em;
          width: 12em;
        }
      }

      .contact {
        top: unset;
        position: relative;
        height: 50em;

        #contact-header {
          font-size: 3em;
          margin: 2em;
        }

        #email-logo {
          position: relative;
          padding-top: 2em;
          transform: translate(-50%, -50%);
          left: 50%;
          width: 9em;
        }

        #email-address {
          font-size: 3em;
          margin-top: 0.5em;
        }

        #linkedin-logo {
          width: 23em;
          top: 13em;
        }

        img {
          padding-top: 0;
        }
      }
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
