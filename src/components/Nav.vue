<template>
  <div class="nav">

    <div ref="menuItems" class="menu-items hidden">
      <router-link id="home-link" to="/">Home</router-link>
      <router-link id="about-link" to="About">About</router-link>
    </div>

    <img alt="navigation menu button" src="../assets/burger.svg" v-on:click="onClick">

  </div>
</template>

<script>
export default {
  name: "Nav",
  methods: {
    onClick: function () {
      const items = this.$refs.menuItems;

      if (items.classList.contains("hidden")) items.classList.remove("hidden")
      else items.classList.add("hidden")
    }
  }
}
</script>

<style scoped lang="scss">

.nav {
  position: absolute;
  right: 0;
  margin: 1em;
  top: 0;

  .menu-items {
    transition: opacity 0.5s ease;
    overflow: hidden;
    opacity: 1;
    float: left;
    margin-top: .3em;

    a {
      padding: 1em;
      color: #fff;
      text-decoration: none;
      font-family: 'Montserrat', sans-serif;
      font-size: 1.6em;
      font-weight: 400;
    }

    &.hidden {
      opacity: 0;
    }
  }
}

</style>