<script setup>
import CardIngradients from './CardIngradients.vue'
</script>

<template>
  <div id="section-03">
    <div class="container">
      <div class="info">
        <h2 class="title">OUR INGRADIENTS</h2>
        <p>
          Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras ullamcorper bibendum bibendum. Duis tincidunt urna non pretium porta. Nam condimentum vitae ligula vel ornare. Phasellus at semper turpis. Nunc eu tellus tortor. Etiam at condimentum nisl, vitae sagittis orci. Donec id dignissim nunc. Donec elit ante, eleifend a dolor et, venenatis facilisis dolor. In feugiat orci odio, sed lacinia sem elementum quis. Aliquam consectetur, eros et vulputate euismod, nunc leo tempor lacus, ac rhoncus neque eros nec lacus. Cras lobortis molestie faucibus.
        </p>
        <a href="#" class="btn">
          <span>OUR SERVICES</span><span class="btn-line"></span>
        </a>
      </div>
      <div class="card-wrap">
        <CardIngradients></CardIngradients>
        <a href="#" class="more-btn">VIEW MORE DIGISALAD’S INGRADIENTS</a>
      </div>
    </div>

    <div class="about">
      <div class="container">
        <div class="character">
          <div class="avatar">
            <img src="../assets/TST1914.jpg" alt="avatar">
          </div>
          <h4 class="name">Tony Ng</h4>
          <div class="position">Founder & Creative Director</div>
        </div>
        <div class="text">
          <div class="icon">
            <img src="../assets/left-quote.png" alt="quote">
          </div>
          <p>
            A great digital work isn’t about designing beautiful pages purely. It is about context - how do we deliver the <span>right experience to the right person at the right time.</span>The most important thing is that your work can engage customers at anytime, anywhere and let users experience an entire amazing digital journey.
          </p>
        </div>
      </div>
    </div>

  </div>
</template>

<style scoped>

#section-03 {
  width: 100%;
  background-color:#26C6D0;
  border-radius: 50px 50px 0 0 ;
  position: relative;
  padding-bottom: 433px;
}
#section-03::before {
  content: '';
  position: absolute;
  inset: 0;
  background-color:#E5E5E5;
  z-index: -1;
}

.info {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: auto;
  padding-top: 216px;
}

.title {
  color:#FFFFFF;
}

.title::before {
  background-image: url(../assets/wave585880.png);
}

.btn {
  width: 294px;
  height: 92px;
  background-color: #585880;
}

.info p {
  max-width: 960px;
  color:#FFFFFF;
}

.card-wrap {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

.more-btn {
  display: inline-block;
  text-decoration: none;
  font-style: normal;
  font-weight: 700;
  font-size: 18px;
  line-height: 22px;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: #FFFFFF;
  position: relative;
  z-index: 1;
}
.more-btn::after {
  content: '';
  position: absolute;
  left: -5px;
  right: -5px;
  bottom: 1px;
  height: 10px;
  background-color:#FFBC58;
  z-index: -1;
}

.about {
  background-color: #ffff;
  border-radius: 0 50px 50px 50px;
  max-width: 1280px;
  height: 598px;
  position: absolute;
  bottom: -299px;
  left: 0;
  z-index: 1;
  display: flex;
  align-items: center;

  background-image: url(../assets/shutterstock_675737842.jpg);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

.about .container {
  display: flex;
  align-items: center;
  justify-content: space-around;
  width: 100%;
  /* margin-left: 25%; */
  /* padding-left: 299px; */
  /* padding-left: 75px; */
  /* padding-top: 299px; */
}

.about .character {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-right: 50px;
}



.about .avatar {
  width: 204px;
  height: 204px;
  border-radius: 50%;
  overflow: hidden;
  margin-bottom: 15%;
}

.about .name {
  font-style: normal;
  font-weight: 700;
  font-size: 20px;
  line-height: 24px;
  text-align: center;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: #FFFFFF;
}

.about .position {
  font-style: italic;
  font-weight: 400;
  font-size: 16px;
  line-height: 16px;
  text-align: center;
  letter-spacing: 2px;
  color: #FFFFFF;
  padding-top: 3%;
}
.about .text {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.about .icon {
  width: 90px;
  height: 90px;
  overflow: hidden;
  margin: 20px;
}

.about p {
  font-style: normal;
  font-weight: 400;
  font-size: 22px;
  line-height: 48px;
  letter-spacing: 2px;
  color: #fff;
  text-align: left;
  max-width: 800px;
}

.about p span {
  color: #FFBC58;
}

</style>
