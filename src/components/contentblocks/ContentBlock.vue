<template>
  <div class="contentBlock">
    <div class="picture" :style="{ 'backgroundImage': 'url(' + require('@/assets/' + picUrl) + ')'}">
      <button v-on:click="btnClick">Click me!</button>
    </div>
    <div class="description"><p><span>{{ title }}</span>{{ msg }}</p></div>
  </div>
</template>

<script>

export default {
  name: 'ContentBlock',
  props: {
    msg: String,
    title: String,
    picUrl: String,
  },
  methods: {
    btnClick: function () {
      alert("suvaline tekst");
    }
  }
}
</script>


<style scoped lang="scss">
.description {
  font-family: Montserrat, sans-serif;
  font-size: 1.1em;
  line-height: 124%;
  font-weight: 400;
  margin: auto;
  width: 80vw;
  float: none;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #FFFFFF;
}

span {
  font-weight: 600;
}

.picture {
  height: 36vh;
  width: 80vw;
  float: none;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 3vh auto 1vh auto;
}

button {
  margin-top: 26vh;
  margin-left: 42vw;
  width: 30vw;
  height: 6vh;
  border-radius: 45px;
  border: none;
  background: #B53D4B;
  font-family: Montserrat, sans-serif;
  font-weight: 500;
  color: #FFF;

}

</style>
