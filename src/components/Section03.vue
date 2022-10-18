<script setup>
</script>

<template>
  <div class="section-03">
    <div class="container">
      <h2 class="title">OUR INGRADIENTS</h2>
      <p>Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras ullamcorper bibendum bibendum. Duis tincidunt urna non pretium porta. Nam condimentum vitae ligula vel ornare. Phasellus at semper turpis. Nunc eu tellus tortor. Etiam at condimentum nisl, vitae sagittis orci. Donec id dignissim nunc. Donec elit ante, eleifend a dolor et, venenatis facilisis dolor. In feugiat orci odio, sed lacinia sem elementum quis. Aliquam consectetur, eros et vulputate euismod, nunc leo tempor lacus, ac rhoncus neque eros nec lacus. Cras lobortis molestie faucibus.</p>
      <a href="#" class="btn"><span>OUR SERVICES</span><span class="btn-line"></span></a>
    
    </div>
  </div>
</template>

<style scoped>
.section-03 {
  width: 100%;
  /* height: 100vh; */
  background-color:#26C6D0;
  border-radius: 50px 50px 0 0 ;
  position: relative;
}
.section-03::before {
  content: '';
  position: absolute;
  inset: 0;
  background-color:#E5E5E5;
  z-index: -1;
}

.container {
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

p {
  color:#FFFFFF;
}

</style>
