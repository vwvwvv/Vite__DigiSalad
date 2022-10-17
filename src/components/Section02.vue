<script setup>
</script>

<template>
  <div class="section-02">
    <div class="container">
      <h2 class="title">ABOUT DIGISALAD</h2>
      <div class="video-container">
        <div class="video">
          <iframe frameborder="0" src="https://www.youtube.com/embed/IeIRJ9jZ5Ro" allowFullScreen="true"></iframe>
        </div>
      </div>
      <p>Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras ullamcorper bibendum bibendum. Duis tincidunt urna non pretium porta. Nam condimentum vitae ligula vel ornare. Phasellus at semper turpis. Nunc eu tellus tortor. Etiam at condimentum nisl, vitae sagittis orci. Donec id dignissim nunc. Donec elit ante, eleifend a dolor et, venenatis facilisis dolor. In feugiat orci odio, sed lacinia sem elementum quis. Aliquam consectetur, eros et vulputate euismod, nunc leo tempor lacus, ac rhoncus neque eros nec lacus. Cras lobortis molestie faucibus.</p>
      <a href="#"><span>VIEW MORE</span><span class="line"></span></a>
      <!-- <div class="btn"><a href="#">VIEW MORE<span class="line"></span></a></div> -->
    </div>
  </div>
</template>

<style scoped>
.section-02 {
  width: 100%;
  /* height: 100vh; */
  background-color:#E5E5E5;
}
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: auto;
}
.video-container {
  max-width: 960px;
  margin: auto;
  padding: 0 80px;
  width: 100%;
  margin-bottom: 30px;
}
.video {
  position: relative;
  height: 0;
  padding-bottom: 56.25%;
  /* margin-bottom: 100px; */
}

.video iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

p {
  width: 960px;
  text-align: center;
  font-weight: 400;
  font-size: 16px;
  line-height: 28px;
  letter-spacing: 1px;
}

a {
  width: 223px;
  height: 86px;
  border-radius: 1px;
  background-color: #26C6D0;
  text-decoration: none;
  margin: 70px;
  font-size: 16px;
  font-weight: 700;
  letter-spacing: 2px;
  color: #ffff;
  display: flex;
  justify-content: center;
  align-items: center;
}

.line {
  display: block;
  width: 52px;
  height: 2px;
  background-color: #ffff;
  margin-left: 15px;
}

/* a::after {
  content: '';
  position: absolute;
  width: 52px;
  height: 2px;
  background-color: #ffff;
  top: 50%;
  right: 0;
} */

/* 
.btn {
    display: block;
    width: 223px;
    height: 86px;
    border-radius: 1px;
    background-color: #26C6D0;
  }

a {
  text-decoration: none;
  font-size: 16px;
  font-weight: 700;
  letter-spacing: 2px;
  color: #ffff;
}

a::after {
  content: '';
  position: absolute;
  width: 50px;
  height: 2px;
  background-color: #ffff;
} */

/* .line {
  width: 50px;
  height: 2px;
  background-color: #ffff;
  display: ;
} */

</style>
