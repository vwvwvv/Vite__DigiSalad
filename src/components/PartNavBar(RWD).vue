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
    const partNavbar = document.querySelector('#part-navbar')
    partNavbar.classList.toggle('stick', window.scrollY > 0)
  })
})


</script>

<template>
  <div id="part-navbar">
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
              <div class="col about-us">
                <div class="wrap">
                  <div class="pic">
                  <img src="../assets/CardIngradients/ingradient_01.png" alt="about-us">
                  </div>
                  <div class="text">
                    <h6>EMPOWERING BRANDS</h6>
                    <h1 class="heading">ABOUT US</h1>
                  </div>
                  <a href="#"></a>
                </div>
              </div>
              <div class="col works">
                <div class="wrap">
                  <div class="pic">
                  <img src="../assets/CardIngradients/ingradient_02.png" alt="about-us">
                  </div>
                  <div class="text">
                    <h6>CASE STUDIES</h6>
                    <h1 class="heading">WORKS</h1>
                  </div>
                  <a href="#"></a>
                </div>
              </div>
            </div>

            <div class="row">
              <div class="col careers">
                <div class="wrap">
                  <div class="pic">
                    <img src="../assets/CardIngradients/ingradient_03.png" alt="about-us">
                  </div>
                  <div class="text">
                    <h6>BE COOL WITH US</h6>
                    <h1 class="heading">CAREERS</h1>
                  </div>
                  <a href="#"></a>
                </div>
              </div>
              <div class="col insights">
                <div class="wrap">
                  <div class="pic">
                    <img src="../assets/CardIngradients/ingradient_11.png" alt="about-us">
                  </div>
                  <div class="text">
                    <h6>OUR STRATEGIES</h6>
                    <h1 class="heading">INSIGHTS</h1>
                  </div>
                  <a href="#"></a>
                </div>
              </div>
            </div>

            <div class="row">
              <div class="col contact">
                <div class="wrap">
                  <div class="text">
                    <h6>START YOUR JOURNEY WITH US</h6>
                    <h1 class="heading">CONTACT</h1>
                  </div>
                  <a href="#"></a>
                </div>
              </div>
              <div class="col services">
                <div class="wrap">
                  <div class="pic">
                  <img src="../assets/CardIngradients/ingradient_10.png" alt="about-us">
                  </div>
                  <div class="text">
                    <h6>AREAS OF EXPERTISE</h6>
                    <h1 class="heading">SERVICES</h1>
                  </div>
                  <a href="#"></a>
                </div>
              </div>
            </div>

        </div>
      </div>
  </div>
</template>

<style scoped>

#part-navbar {
  width: 100%;
  height: 100px;
  background-color: transparent;
  padding-left: 60px;
  padding-right: 60px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: fixed;
  z-index: 9999;
  transition: 0.5s;
}

#part-navbar.stick {
  background-color:rgba(255,255,255,1);
}

#part-navbar .logo {
  /* width: 120px; */
  height: 54px;
  opacity: 0;
}

#part-navbar.stick .logo {
  opacity: 1;
}

#part-navbar .menu {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

#part-navbar button {
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

#part-navbar.stick .hamburger-line,
#part-navbar.stick .hamburger::before,
#part-navbar.stick .hamburger::after {
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

/* ------------------------ */
/* 漢堡選單.open */
/* ------------------------ */
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
  /* height: 100vh; */
  overflow: hidden;
  z-index: 1;
  /* background: linear-gradient(180deg, #585880 3.61%, #26C6D0 95.7%); */
  /* background: linear-gradient(180deg, rgba(88, 88, 128, 0.5) 3.61%, rgba(38, 198, 208, 0.5) 95.7%); */
  background: linear-gradient(180deg, rgba(88, 88, 128, 0.5) 3.61%, rgba(38, 198, 208, 0.5) 95.7%), url(@/assets/BG.jpg);

  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
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
  /* padding-top: 100px; */
  /* padding-top: 25%; */
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 80%;
  /* height: 0; */
  /* position: absolute;
  left: 0;
  right: 0; */
  height: 100%;

}

.row {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 32%;
}

.col {
  border-radius: 30px;
  margin: 5%;
  position: relative;
}

.row:nth-child(2) {
  width: 25%;
  justify-content: space-between;
}

.row:nth-child(3) {
  flex-direction: column-reverse;
}
.wrap {
  display: flex;
  align-items: center;
  position: absolute;
  inset: 0;
  z-index: 20;
  padding: 50px 25px;
}
.wrap a {
  position: absolute;
  inset: 0;
  text-decoration: none;
}
.col:first-child {
  /* max-width: 380px; */
  /* height: 210px; */
  /* width: 29%; */
  padding-bottom: 55%;
  width: 100%;
}

.col:last-child {
  /* max-width: 380px; */
  /* width: 29%; */
  /* height: 320px; */
  padding-bottom: 84%;
  width: 100%;
}

/* ------------------------ */
/* about */
/* ------------------------ */
.about-us {
  /* background-color: #26C6D0; */
  background-color: rgba(38, 198, 208, 0.9);
  background-blend-mode: multiply;
  background-image: url(../assets/menu01.jpg);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  transition: all 0.5s;
}

.about-us:hover {
  background-color: rgba(27, 161, 170, 0.9);
  background-size: 150%;
  box-shadow: 0 0 10px rgba(0, 0, 0, .5);
}

/* ------------------------ */
/* works */
/* ------------------------ */
.works {
  /* background-color: #EE6C8A; */
  background-color: rgba(238, 108, 138, 0.9);
  background-blend-mode: multiply;
  background-image: url(../assets/menu02.jpg);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  transition: all 0.5s;
}
.works:hover {
  background-color: rgb(203, 89, 115);
  background-size: 150%;
  box-shadow: 0 0 10px rgba(0, 0, 0, .5);
}
.works .wrap {
  align-items: flex-end;
}


.careers .wrap,
.insights .wrap,
.services .wrap {
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-end;
}



/* ------------------------ */
/* careers */
/* ------------------------ */
.row:nth-child(2) .careers {
  /* width: 290px; */
  /* width: 44%; */
  /* height: 430px; */
  padding-bottom: 148%;
  width: 100%;

  background-color: rgba(230, 169, 78, 0.9);
  background-blend-mode: multiply;
  background-image: url(../assets/menu03.jpg);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  transition: all 0.5s;
}
.row:nth-child(2) .careers:hover {
  background-color: rgba(149, 104, 40, 0.9);
  background-size: 150%;
  box-shadow: 0 0 10px rgba(0, 0, 0, .5);
}
.careers .pic {
  height: 60px;
  padding-bottom: 20px;
}

/* ------------------------ */
/* insights */
/* ------------------------ */
.row:nth-child(2) .insights {
  /* width: 44%; */
  /* width: 290px; */
  /* height: 282px; */
  /* background-color: #26D0A8; */
  padding-bottom: 97%;
  width: 100%;
  background-color: rgba(38, 208, 168, 0.9);
  background-blend-mode: multiply;
  background-image: url(../assets/menu04.jpg);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  transition: all 0.5s;
}
.row:nth-child(2) .insights:hover {
  background-color: rgba(23, 147, 118, 0.9);
  background-size: 150%;
  box-shadow: 0 0 10px rgba(0, 0, 0, .5);
}
.insights .pic {
  height: 79px;
  padding-bottom: 20px;
}



/* ------------------------ */
/* services */
/* ------------------------ */
.services {
  /* background-color: #585880; */
  background-color: rgba(88, 88, 128, 0.9);
  background-blend-mode: multiply;
  background-image: url(../assets/menu05.jpg);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  transition: all 0.5s;
}

.services:hover {
  background-color: rgba(47, 47, 81, 0.9);
  background-size: 150%;
  box-shadow: 0 0 10px rgba(0, 0, 0, .5);
}

.services .pic {
  height: 79px;
  padding-bottom: 20px;
}

/* ------------------------ */
/* contact */
/* ------------------------ */
.contact {
  background-color: rgba(255,255,255,0.9);
  transition: all 0.5s;
} 
.contact:hover {
  background-color: rgba(224, 224, 224, 0.9);
  box-shadow: 0 0 10px rgba(0, 0, 0, .5);
}


/* ------------------------ */
/* 差異設定 */
/* ------------------------ */
.heading {
  font-style: normal;
  font-weight: 700;
  font-size: 32px;
  line-height: 39px;
  letter-spacing: 3.5px;
  color: #FFFFFF;
  position: relative;
  display: inline-block;
}

.heading::after {
  content: '';
  position: absolute;
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background-color: #EE6C8A;
  bottom: 5px;
  right: -20px;
}

.works .heading::after {
  background-color: #26C6D0;
} 

h6 {
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 19px;
  letter-spacing: 1.8px;
  color: #FFFFFF;
  padding-bottom: 10px;
}

.contact .heading {
  color: #26C6D0;
}

.contact h6 {
  color: #262626;
}


.pic {
  padding-right: 20px;
}

@media (max-width: 1200px) {
  .overlays .container {
    width: 100%;
  }
  .heading {
    font-size: 25px;
  }
  .pic {
    max-width: 200px;
  }
}

@media (max-width: 768px) {
  .heading {
    font-size: 25px;
  }
  .overlays .container {
    flex-direction: column;
    height: 90vh;
    margin-top: 100px;
    display: block;
  }

  .row,
  .row:nth-child(2) {
    width: 100%;
    height: 30%;
    margin: 0;
    padding: 0;
    justify-content: flex-start;
  }

   .col:first-child,
   .col:last-child {
    width: 100%;
    padding: 0;
    margin: 8px;
    height: 100%;
   } 

   .row:nth-child(2) .col {
      width: 100%;
      padding: 0;
   }

  .wrap,
   .works .wrap,
  .careers .wrap,
  .insights .wrap,
  .services .wrap {
    flex-direction: row;
    justify-content:flex-start;
    align-items: center;
  }

  h6  {
    padding: 0;
  }

  .pic {
    width: 50px;
    padding: 5px;
  }

  .text {
    margin-left: 20px;
  }

}

</style>
