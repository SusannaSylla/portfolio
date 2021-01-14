<template>
  <div class="header-content">
    <p class="title"><span class="nb">Software developer</span><span class="tint-red"> /</span><br><span class="tab">Student</span>
    </p>
    <p class="portfolio-title">PORTFOLIO</p>
    <img class="down-arrow bounce" alt="scroll down image" src="../assets/down.svg">

  </div>
</template>

<script>

export default {
  name: "HeaderContent",
}
</script>

<style lang="scss" scoped>

.header-content {
  position: absolute;
  top: 65%;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  height: 35%;
}

.portfolio-title {
  padding: 0;
  color: #B53D4B;
  font-family: Montserrat, sans-serif;
  font-size: 14vw;
  font-weight: 500;
  text-transform: uppercase;
}

.title {
  position: absolute;
  top: -3em;
  left: 1em;
  padding: 0;
  color: #FFF;
  font-family: Montserrat, sans-serif;
  font-size: 8vw;
  font-weight: 400;
  line-height: 1.2em;
}

.down-arrow {
  position: absolute;
  margin-bottom: -1.5em;
  bottom: 0;
}

.nb {
  white-space: nowrap;
}

.tint-red {
  color: #B53D4B;
}

.tab {
  display: inline-block;
  margin-left: 6.7em;
}
@keyframes bounce {
  0%, 20%, 50%, 80%, 100% {
    transform: translateY(0);
  }
  40% {
    transform: translateY(-30px);
  }
  60% {
    transform: translateY(-15px);
  }
}

.down-arrow.bounce {
  animation: bounce 2s infinite;
}

</style>