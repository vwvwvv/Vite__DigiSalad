<script setup>
import{ reactive } from 'vue'
const BrandLogos = reactive([
  { img: new URL("../assets/BrandLogo/c001.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c002.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c003.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c004.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c005.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c006.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c007.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c008.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c009.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c010.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c011.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c012.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c013.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c014.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c015.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c016.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c017.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c018.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c019.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c020.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c021.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c022.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c023.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c024.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c025.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c026.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c027.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c028.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c029.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c030.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c031.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c032.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c033.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c034.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c035.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c036.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c037.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c038.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c039.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c040.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c041.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c042.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c043.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c044.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c045.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c046.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c047.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c048.png", import.meta.url).href },
  { img: new URL("../assets/BrandLogo/c049.png", import.meta.url).href }
])

</script>

<template>
  <div id="card-BrandLogos" >
    <div class="brand-logo" v-for="BrandLogo in BrandLogos" :key='BrandLogo'>
      <div class="pic">
        <a href="#">
          <img :src="BrandLogo.img" alt="">
        </a>
      </div>
    </div>
  </div>
</template>

<style scoped>

#card-BrandLogos{
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  padding-top: 60px;
  padding-bottom: 100px;
}
.brand-logo {
    width: 14%;
    padding: 25px;
}


</style>
