<template>
  <div id="app">
    <router-view>
<!--        <div id="nav">
          <router-link to="/">Home</router-link> |
          <router-link to="/about">About</router-link>
        </div>-->
    </router-view>
  </div>
</template>

<style lang="scss">

* {
  margin: 0;
  padding: 0;
}

body {
  width: 100%;
  box-sizing: border-box;
  overflow-y: scroll;
  background-color: #495562;
  overflow-x: hidden;
}

/deep/ .header {
  .nav{
    margin: 3em 5em;
  }
  .top-name{
    margin: 2em 0 0 3em;

    span{
      font-size: 2.8rem;
    }
    .tab{
      margin-left: 110px;
    }
    .full-name{
      font-size: 1.8rem;
    }
    .rose-line{
      width:  13em;
      height: 0.40em;
      margin: 0.3em 0 0.4em 0;

      &.first {
        margin-left: 4.5em;
      }

      &.second {
        margin-top: .2em;
        margin-left: -.9em;

      }
    }
  }
}
</style>
