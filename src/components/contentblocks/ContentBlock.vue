<template>
  <div class="contentBlock">

    <div class="picture" :style="{ 'backgroundImage': 'url(' + require('@/assets/' + data.picUrl) + ')'}">
      <button v-on:click="btnClick(data.btnUrl)">Click here!</button>
    </div>

    <div class="description">
      <p v-html="data.title + data.msg"></p>
    </div>

  </div>
</template>

<script>

export default {
  name: 'ContentBlock',
  props: {
    data: Object,
  },
  methods: {
    btnClick: function (btnUrl) {
      window.location = btnUrl;
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
  padding: .5em 0 1em 0;
}

data.title {
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
  background-repeat: no-repeat;
  background-size: 80vw 36vh;
}

button {
  margin-top: 15em;
  margin-left: 12em;
  width: 10em;
  height: 3.4em;
  border-radius: 45px;
  border: none;
  background: #B53D4B;
  font-family: Montserrat, sans-serif;
  font-weight: 500;
  color: #FFF;
  outline: none;
}

button:active {
  background: #91313c;
}

@media only screen and (min-width: 768px) {
  button {
    margin-left: 20em;
    font-size: 1.5rem;
    margin-right: 2em;
  }
}
</style>
