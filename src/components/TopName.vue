<template>
  <router-link to="/">

    <div class="top-name">
      <p class="full-name"><span>S</span>usanna<br><span class="tab">S</span>aadi</p>
      <div class="rose-line first"></div>
      <div class="rose-line second"></div>
    </div>

  </router-link>
</template>

<script>
export default {
  name: "TopName"
}
</script>

<style scoped lang="scss">
.top-name {
  position: absolute;
  margin: 1em 0.9em;
  top: 0;
}

span {
  font-size: 1.3rem;
}

.tab {
  display: inline-block;
  margin-left: 70px;
}

.full-name {
  padding: 0;
  color: #FFF;
  font-family: Montserrat, sans-serif;
  font-size: 1rem;
  font-weight: 500;
  text-transform: uppercase;
}

.rose-line {
  height: 0.21em;
  width: 6.7em;
  background: #B53D4B;

  &.first {
    margin-left: 2em;
  }

  &.second {
    margin-top: .2em;
    margin-left: -.3em;

  }
}

</style>