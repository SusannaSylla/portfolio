<template>
  <div class="content">
    <ContentBlock :data="contentConfig[0]"></ContentBlock>
    <ContentBlock :data="contentConfig[1]"></ContentBlock>
    <ContentBlock :data="contentConfig[2]"></ContentBlock>
  </div>
</template>

<script>
import ContentBlock from '@/components/contentblocks/ContentBlock.vue'

export default {
  name: 'MainContent',
  components: {
    ContentBlock,
  },
  data: function () {
    return {
      contentConfig: [
        {
          btnUrl: "https://susannasaadi.computer/slot-game/",
          picUrl: "screenshotSlotGame.jpg",
          title: "<b>Slot Game</b> ",
          msg: `started when I had to do an exam for BCS web application development training certificate (see on <a href="#">about</a> page). Now it's a little redesigned to fit the style of the portfolio. I built this page with pure HTML5, JS, CSS.
              My first big project I designed, built and finished alone. Take a closer look at the page and play the fun game by clicking the button!`,
        },
        {
          btnUrl:"https://susannasaadi.computer/music-app/",
          picUrl: "screenshotMusicApp.jpg",
          title: "<b>Music App </b>",
          msg: `is my first Vue.js test page where you can listen to music. I did it according to the tutorial found on youtube and looking back, it was quite horrible code,
          but vue.js was easy to learn and I loved it. Now I finished my portfolio in the Vue.js framework, which hopefully has better code quality. You can explore more and listen to music by clicking the button!`,
        },
        {
          btnUrl: "/",
          picUrl: "screenshotComingSoon.jpg",
          title: "<b>Coming soon </b>",
          msg: ``,
        },
      ]
    }
  },
  props: {
    msg: String
  },
}
</script>


<style scoped lang="scss">
.content {
  padding-top: 2vh;
  padding-bottom: 4vh;
  background-image: linear-gradient(#020B17, #062041);
}

</style>
