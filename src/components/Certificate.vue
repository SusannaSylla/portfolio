<template>
  <div class="certificate">
    <p class="certificateHeader" id="CertificateH1">Check out my certificate:</p>
    <a class="lightbox" href="#certificate">
      <img src="../assets/certificateZoom.png" alt="certificate">
    </a>
    <div class="lightbox-target" id="certificate">
      <img src="../assets/certificate.png" alt="certificate">
      <a class="lightbox-close" href="#certificateH1"></a>
    </div>
    <p class="info">(Zoom in by clicking on the picture)</p>
  </div>
</template>

<script>
export default {
  name: "Certificate"
}
</script>

<style scoped>

.certificateHeader {
  color: #FFFFFF;
  padding: 10% 2% 5% 2%;
  font-size: 1.75em;
  font-family: 'Montserrat', sans-serif;
  font-weight: 500;
}

a.lightbox img {
  border: 1px solid white;
  box-shadow: 0 0 8px rgba(0, 0, 0, .3);
  margin: auto;
  width: 100%;
}

/* Styles the lightbox, removes it from sight and adds the fade-in transition */

.lightbox-target {
  position: fixed;
  top: -100%;
  width: 100%;
  background: rgba(0, 0, 0, .7);
  opacity: 0;
  transition: opacity .5s ease-in-out;
  overflow: hidden;
  z-index: 90;
}

/* Styles the lightbox image, centers it vertically and horizontally, adds the zoom-in transition and makes it responsive using a combination of margin and absolute positioning */

.lightbox-target img {
  margin: auto;
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  max-height: 0%;
  max-width: 0%;
  border: 1px solid white;
  box-shadow: 0 0 8px rgba(0, 0, 0, .3);
  box-sizing: border-box;
  transition: .5s ease-in-out;
}

/* Styles the close link, adds the slide down transition */

a.lightbox-close {
  display: block;
  width: 15%;
  height: 8%;
  box-sizing: border-box;
  background: white;
  color: black;
  text-decoration: none;
  position: absolute;
  top: -8%;
  right: 0;
  transition: .5s ease-in-out;
}

/* Provides part of the "X" to eliminate an image from the close link */

a.lightbox-close:before {
  content: "";
  display: block;
  height: 30px;
  width: 1px;
  background: black;
  position: absolute;
  left: 26px;
  top: 10px;
  transform: rotate(45deg);
}

/* Provides part of the "X" to eliminate an image from the close link */

a.lightbox-close:after {
  content: "";
  display: block;
  height: 30px;
  width: 1px;
  background: black;
  position: absolute;
  left: 26px;
  top: 10px;
  transform: rotate(-45deg);
}

/* Uses the :target pseudo-class to perform the animations upon clicking the .lightbox-target anchor */

.lightbox-target:target {
  opacity: 1;
  top: 0;
  bottom: 0;
}

.lightbox-target:target img {
  max-height: 100vh;
  max-width: 100vw;
}

.lightbox-target:target a.lightbox-close {
  top: 0;
}

.info {
  color: #FFFFFF;
  position: absolute;
  font-weight: 200;
  font-family: 'Montserrat', sans-serif;
  font-size: 1em;
  left: 13.5%;
}


</style>