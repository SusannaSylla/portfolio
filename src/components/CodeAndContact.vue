<template>
  <div class="codeNContact">
    <div class="code">
      <p>Check out this portfolio's code:</p>
      <a href="https://github.com/susannasaadi/portfolio" target="_blank">
        <img src="../assets/githubLogo.svg" alt="github logo" class="github-logo">
      </a>
    </div>
    <div class="contact">
      <p class="contact-header">Contact me!</p>
      <a href="mailto:susannasaadi@gmail.com" target="_blank">
        <img src="../assets/EmailLogo.svg" alt="email logo" class="email-logo">
      </a>
      <p class="email-address">susannasaadi@gmail.com</p>
      <a href="https://www.linkedin.com/in/susanna-s-78b38a1aa/" target="_blank">
        <img src="../assets/linkedinLogo.svg" class="linkedin-logo">
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "CodeAndContact"
}
</script>

<style scoped>
.codeNContact {
  color: #FFFFFF;
  font-family: 'Montserrat', sans-serif;

}

.code {
  background-color: #495562;
  top: 243%;
  width: 100vw;
  height: 30%;
  position: absolute;
}

.code p {
  padding-top: 2%;
  text-align: center;
  font-weight: 500;
  font-size: 1.7em;
}

.code img {
  /*padding: 37% 0 0 100%;*/
  position: absolute;
  left: 50%;
  top: 9em;
  width: 120px;
  transform: translate(-50%, -50%);
}

.contact {
  top: 274%;
  position: absolute;
  width: 100vw;
}

.contact p {
  text-align: center;
}

.contact-header {
  font-size: 2em;
  font-weight: 500;
}

.email-address {
  margin-top: -70px;
  font-weight: 300;
  /*font-size: 1.6em;*/
  font-size: calc(.5em + 4vw);
}

.contact img {
  position: relative;
  transform: translate(-50%, -50%);
  left: 50%;
}
.email-logo{
  width: 100px;
  padding-top: 100px;
}
.linkedin-logo {
  width: 200px;
  padding-top: 80px;
}
</style>
