<template>
  <div class="codeNContact">
    <div class="code">
      <p>Check out this portfolio's code:</p>
      <a href="www.https://github.com/susannasaadi/portfolio">
        <img src="../assets/githubLogo.png" alt="github logo">
      </a>
    </div>
    <div class="contact">
      <p id="contact-header">Contact me!</p>
      <a href="mailto:susannasaadi@gmail.com">
        <img src="../assets/EmailLogo.png" alt="email logo" id="email-logo">
      </a>
      <p id="email-address">susannasaadi@gmail.com</p>
      <a href="https://www.linkedin.com/in/susanna-s-78b38a1aa/">
        <img src="../assets/linkedinLogo.png" id="linkedin-logo">
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
  top: 70%;
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

#contact-header {
  font-size: 2em;
  font-weight: 500;
}

/*#email-logo {
  padding-top: 20%;
}*/

#email-address {
  margin-top: -13%;
  font-weight: 300;
  /*font-size: 1.6em;*/
  font-size: calc(.5em + 4vw);
}

/*
#linkedin-logo {
  padding-top: 20%;
}
*/

.contact img {
  position: relative;
  padding-top: 20%;
  transform: translate(-50%, -50%);
  left: 50%;
}
</style>
