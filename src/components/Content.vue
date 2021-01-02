<template>
  <div class="content">

    <ContentBlock></ContentBlock>
    <ContentBlock></ContentBlock>
    <ContentBlock></ContentBlock>

  </div>
</template>

<script>
import ContentBlock from '@/components/contentblocks/ContentBlock.vue'

export default {
  name: 'Content',
  components: {
    ContentBlock,
  },
  props: {
    msg: String
  },
}
</script>


<style scoped lang="scss">
.content{
  padding-top: 2vh;
  padding-bottom: 4vh;
  background-image: linear-gradient(#020B17,#062041);
}
</style>
