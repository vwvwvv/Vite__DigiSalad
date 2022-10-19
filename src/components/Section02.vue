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
      <a href="#" class="btn"><span>VIEW MORE</span><span class="btn-line"></span></a>

    </div>

    <div class="awards">
      <div class="container">
        <div class="text">
          <h2 class="title">AWARDS</h2>
          <p>Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras ullamcorper bibendum bibendum. Duis tincidunt urna non pretium porta. Nam condimentum vitae ligula vel ornare. Phasellus at semper turpis. Nunc eu tellus tortor. Etiam at condimentum nisl, vitae sagittis orci. Donec id dignissim nunc.</p>
        </div>
        <div class="pic">
          <div class="row">
            <div class="col">
              <img src="../assets/image5.png">
            </div>
            <div class="col">
              <img src="../assets/image5.png">
            </div>
          </div>
          <div class="row">
            <div class="col">
              <img src="../assets/image5.png">
            </div>
            <div class="col">
              <img src="../assets/image5.png">
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

</template>

<style scoped>
.section-02 {
  width: 100%;
  /* height: 100vh; */
  background-color:#E5E5E5;
  position: relative;
}
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: auto;
  padding-bottom: 216px;
}

p {
  max-width: 960px;
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

.btn {
  width: 223px;
  height: 86px;
}

.awards {
  background-color: #ffff;
  border-radius: 50px 0 50px 50px;
  /* width: 100%; */
  width: 1280px;
  height: 432px;
  position: absolute;
  bottom: -216px;
  right: 0;
  z-index: 1;
  display: flex;
  align-items: center;
}

.awards .container {

  flex-direction: row;
  width:100%;
  height: 100%;
  padding-left: 75px;
  padding-right: 230px;
  padding-top: 216px;
}


.awards .text {
  width: 50%;
  margin-right: 50px;
}
.awards p {
  text-align: left;
  font-size: 16px;
  font-weight: 400;
  line-height: 28px;
  letter-spacing: 1px;
  color: #262626;
  margin-top: 50px;
}

.awards .title {
  display: inline-block;
  margin: 0;
}



.awards .pic {
  width: 80%;
  display: flex;
  flex-direction: column;
}

.awards .row {
  display: flex;
  justify-content: space-around;
}


</style>
