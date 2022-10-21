<script setup>
</script>

<template>
  <div id="section-01">
    <div class="container">
      <div class="digital-agency">
        <div class="line"></div>
        <h6>DIGITAL AGENCY</h6>
      </div>
      <div class="content">
        <h1 class="logo">
          <img src="../assets/logoW.png" alt="logo">
        </h1>
        <h2>WE CREATE<br/>AMAZING<br/><span class="f">DIGITAL EXPERIENCES</span></h2>
      </div>

    </div>
    <div class="taste">
      <div class="pic">
        <img src="../assets/te.png" alt="taste">
      </div>
      <h6>TASTE US NOW!</h6>
      <div class="indicator-line"></div>
    </div>


  </div>
</template>

<style scoped>
#section-01 {
  width: 100%;
  height: 100%;
  /* max-height: 900px; */
  background-image: url(@/assets/BG.jpg);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  border-radius: 0 0 50px 50px;
}
.container {
  position: relative;
  max-width: 1440px;
}
.digital-agency  {
  display: flex;
  align-items: center;
  position: absolute;
  
  transform-origin: right top;
  transform: rotate(-90deg);
  top: 249px;
  left: -228.5px;
}
.digital-agency .line {
  width: 113px;
  height: 2px;
  background-color: #fff ;
  margin-right: 24px;
}

.digital-agency h6 {
  font-size: 16px;
  font-weight: 700;
  line-height: 20px;
  letter-spacing: 2px;
  color: #fff;
}


#section-01 .content {
  position: absolute;
  top: 181px;
  left: 220px;
  text-shadow: 0 0 20px rgba(0,0,0,0.5);
  z-index: 1;
}

#section-01 .logo {
  width: 200px;
  margin-bottom: 5%;
}

#section-01 h2 {
  font-weight: 700;
  font-size: 38px;
  color: #fff;
  line-height: 70px;
  letter-spacing: 10px;
}

.content:before {
  content: '';
  position: absolute;
  bottom: 17px;
  left: -5px;
  right: 5px;
  background-color:#26C6D0;
  display: inline-block;
  height: 10px;
  z-index: -1;
}

.content::after {
  content: '';
  position: absolute;
  bottom: 20px;
  right: -15px;
  background-color:#EE6C8A;
  width: 10px;
  height: 10px;
  border-radius: 50%;
  z-index: -1;
}
.taste {
  position: absolute;
  bottom: 0;
  left: 50%;
  transform: translateX(-50%);
  display: flex;
  flex-direction: column;
  align-items: center;
  z-index: 1;
  cursor: pointer;
}
.taste .pic {
  width: 65px;
  height: 65px;
  border-radius: 50%;
  overflow: hidden;
}

.taste h6 {
  font-style: normal;
  font-weight: 700;
  font-size: 14px;
  line-height: 17px;
  letter-spacing: 2px;
  text-transform: uppercase;
  text-align: center;
  color: #FFFFFF;
  padding-top: 10px;
  padding-bottom: 30px;
}

.taste .indicator-line {
  width: 1px;
  height: 50px;
  background-color: #fff;
}

</style>
