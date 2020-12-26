<template>
  <div class="header">

    <TopName></TopName>

    <div class="nav">
      <img alt="navigation menu button" src="../assets/burger.svg">
    </div>

    <HeaderImage></HeaderImage>
    <HeaderContent></HeaderContent>

  </div>
</template>

<script>
import TopName from '@/components/TopName.vue'
import HeaderImage from '@/components/HeaderImage.vue'
import HeaderContent from '@/components/HeaderContent.vue'

export default {
  name: 'Header',
  components: {
    TopName,
    HeaderImage,
    HeaderContent,
  },
  props: {
    msg: String
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
