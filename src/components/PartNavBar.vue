<script setup>
import { onMounted, onUnmounted } from 'vue'

// document.addEventListener("DOMContentLoaded", function(){
//   const hamburger = document.querySelector('.hamburger')
//   const overlays = document.querySelector('.overlays')
//   const open = function() {
//     overlays.classList.toggle('open')
//   }
//   hamburger.addEventListener('click',open)
// })


onMounted(() => {
  const hamburger = document.querySelector('.hamburger')
  const overlays = document.querySelector('.overlays')

  hamburger.addEventListener('click', function() {
    overlays.classList.toggle('open')
    hamburger.classList.toggle('open')
  })

  window.addEventListener('scroll', function() {
    const partNavbar = document.querySelector('.part-navbar')
    partNavbar.classList.toggle('stick', window.scrollY > 0)
  })
})


</script>

<template>
  <div class="part-navbar">
    <h1 class="logo">
      <a href="#">
        <img src="../assets/logoO.png" alt="logo">
      </a>
    </h1>
    <div class="menu">
      <button type="button">START YOUR PROJECT</button>
      <div class="hamburger">
          <span class="hamburger-line"></span>
      </div>
    </div>
    
    <div class="overlays">
        <h1 class="logo2">
          <a href="#">
            <img src="../assets/logoW.png" alt="logo">
          </a>
        </h1>
        <div class="container">
          <div class="row">
            <div class="col"></div>
            <div class="col"></div>
          </div>
          <div class="row">
            <div class="col">about us</div>
            <div class="col">WORKS</div>
          </div>
          <div class="row">
            <div class="col"></div>
            <div class="col"></div>
          </div>
        </div>
      </div>
  </div>
</template>

<style scoped>
.part-navbar {
  width: 100%;
  height: 100px;
  background-color: transparent;
  padding-left: 60px;
  padding-right: 60px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: relative;
  transition: 0.5s;
}

.part-navbar.stick {
  background-color:rgba(255,255,255,1);
}

.part-navbar .logo {
  /* width: 120px; */
  height: 54px;
  opacity: 0;
}

.part-navbar.stick .logo {
  opacity: 1;
}

.part-navbar .menu {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.part-navbar button {
  width: 200px;
  height: 40px;
  border-radius: 24px;
  border: 0;
  background:linear-gradient(90deg, #4EE5EA 3.94%, #26D0A8 94.73%);
  font-style: normal;
  font-weight: 700;
  font-size: 14px;
  line-height: 17px;
  letter-spacing: 1.2px;
  color: #FFFFFF;
  cursor: pointer;
}

/* ------------------------ */
/* 漢堡選單 */
/* ------------------------ */
.hamburger {
  cursor: pointer;
  position: relative;
  width: 30px;
  height: 22px;
  z-index: 9999;
  margin-left: 50px;
  
}

.hamburger-line,
.hamburger::before,
.hamburger::after{
  display: block;
  width: 100%;
  height: 4px;
  background-color: #FFFF;
  border-radius: 100px;
  position: absolute;
  transition: 0.2s;
}

.part-navbar.stick .hamburger-line,
.part-navbar.stick .hamburger::before,
.part-navbar.stick .hamburger::after {
  background-color:#414042;
}

.hamburger-line {
  top: 50%;
  transform: translateY(-50%);
}

.hamburger::before {
  content: '';
  top: 0;
}

.hamburger::after {
  content: '';
  bottom: 0;
  right: 0;
  width: 80%;
}

.open .hamburger-line { display: none;}

.open.hamburger::before,
.open.hamburger::after {
  top: 50%;
  transform: translateY(-50%);
  background-color:rgba(255,255,255,1);
}
.open.hamburger::before {

  transform: rotate(45deg);
}
.open.hamburger::after {
  width: 100%;
  transform: rotate(-45deg);
}


/* ------------------------ */
/* 滿版菜單 */
/* ------------------------ */
.overlays {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 0;
  overflow: hidden;
  z-index: 1;
  /* background: linear-gradient(180deg, #585880 3.61%, #26C6D0 95.7%); */
  /* background: linear-gradient(180deg, rgba(88, 88, 128, 0.5) 3.61%, rgba(38, 198, 208, 0.5) 95.7%); */
  background: linear-gradient(180deg, rgba(88, 88, 128, 0.5) 3.61%, rgba(38, 198, 208, 0.5) 95.7%), url(@/assets/BG.jpg);

  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  /* border-radius: 0 0 50px 50px; */
}
.overlays.open {
  height: 100vh;
  overflow-y: hidden;
}

.logo2 {
  position: absolute;
  height: 54px;
  opacity: 1;
  padding-left: 60px;
  top: 22px;
}
.overlays .container {
padding-top: 100px;
padding-bottom: 100px;
display: flex;
justify-content: space-around;
align-items: center;
}

.row {
  display: flex;
  flex-direction: column;

}
.col {
  border-radius: 30px;
  margin-bottom: 50px;
}

.row:nth-child(2) {
  justify-content: space-between;
}

.row:nth-child(3) {
  flex-direction: column-reverse;
}

.col:first-child {
  width: 380px;
  height: 210px;
  
}

.col:last-child {
  width: 380px;
  height: 320px;
  
}

.row:nth-child(1) .col:first-child {
  background-color: #26C6D0;
}

.row:nth-child(1) .col:last-child {
  background-color: #EE6C8A;
}

.row:nth-child(2) .col:first-child {
  width: 290px;
  height: 430px;
  background-color: #E6A94E;
}

.row:nth-child(2) .col:last-child {
  width: 290px;
  height: 282px;
  background-color: #26D0A8;
}

.row:nth-child(3) .col:first-child {

  background-color: #FFFFFF;
}

.row:nth-child(3) .col:last-child {
  background-color: #585880;
}
</style>
