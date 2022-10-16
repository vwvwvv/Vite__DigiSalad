<script setup>
</script>

<template>
  <div class="section-02">
    <div class="container">
      <h2 class="title">ABOUT DIGISALAD</h2>
      <div class="video">
        <iframe frameborder="0" src="https://www.youtube.com/embed/IeIRJ9jZ5Ro" allowFullScreen="true"></iframe>
      </div>
      <p>Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras ullamcorper bibendum bibendum. Duis tincidunt urna non pretium porta. Nam condimentum vitae ligula vel ornare. Phasellus at semper turpis. Nunc eu tellus tortor. Etiam at condimentum nisl, vitae sagittis orci. Donec id dignissim nunc. Donec elit ante, eleifend a dolor et, venenatis facilisis dolor. In feugiat orci odio, sed lacinia sem elementum quis. Aliquam consectetur, eros et vulputate euismod, nunc leo tempor lacus, ac rhoncus neque eros nec lacus. Cras lobortis molestie faucibus.</p>
      <a href="#">VIEW MORE</a>
    </div>
  </div>
</template>

<style scoped>
.section-02 {
  width: 100%;
  height: 100%;
  background-color:#E5E5E5;
}
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.video {
  position: relative;
  width: 100%;
  height: 0;
  padding-bottom: 56.25%;
}

.video iframe {
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  width: 960px;
  height: 544px;
}

</style>
