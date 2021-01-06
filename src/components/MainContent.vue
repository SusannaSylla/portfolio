<template>
  <div class="content">

    <ContentBlock picUrl="flowers.jpg" title="Lorem Ipsum"
                  msg=" In ac odio luctus, aliquam nibh nec, venenatis odio. Duis commodo arcu sed ex blandit, id fringilla augue pulvinar. Sed egestas, dui ut finibus maximus, ante augue euismod nisi, nec fermentum ligula enim non felis."></ContentBlock>
    <ContentBlock picUrl="face.png" title="Lorem Ipsum"
                  msg=" In ac odio luctus, aliquam nibh nec, venenatis odio. Duis commodo arcu sed ex blandit, id fringilla augue pulvinar. Sed egestas, dui ut finibus maximus, ante augue euismod nisi, nec fermentum ligula enim non felis."></ContentBlock>
    <ContentBlock picUrl="circles.svg" title="Lorem Ipsum"
                  msg=" In ac odio luctus, aliquam nibh nec, venenatis odio. Duis commodo arcu sed ex blandit, id fringilla augue pulvinar. Sed egestas, dui ut finibus maximus, ante augue euismod nisi, nec fermentum ligula enim non felis."></ContentBlock>

  </div>
</template>

<script>
import ContentBlock from '@/components/contentblocks/ContentBlock.vue'

export default {
  name: 'MainContent',
  components: {
    ContentBlock,
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
