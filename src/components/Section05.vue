<script setup>
</script>

<template>
   <div id="section-05">
      <div class="container">
         <button type="button" class="arrow left"></button>
         <div class="view">
            <div class="pic">
               <img src="../assets/LP_fb_01.jpg" alt="LP">
            </div>
            <a href="#" class="btn"><span>VIEW PROJECT</span><span class="btn-line"></span></a>
         </div>

         <div class="text">
            <h5>HIGHLIGHTED SHOWCASE</h5>
            <h1 class="title">LP CLUB MOBILE APP</h1>
            <p>Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras ullamcorper bibendum bibendum. Duis tincidunt urna non pretium porta. Nam condimentum vitae ligula vel ornare. Phasellus at semper turpis. Nunc eu tellus tortor. Etiam at condimentum nisl, vitae sagittis orci. Donec id dignissim nunc. Donec elit ante, eleifend a dolor et, venenatis facilisis dolor. In feugiat orci odio, sed lacinia sem elementum quis. Aliquam consectetur, eros et vulputate euismod, nunc leo tempor lacus, ac rhoncus neque eros nec lacus. Cras lobortis molestie faucibus.</p>
         </div>
         <button type="button" class="arrow right"></button>
         <div class="page">
            <div class="number">01</div>
            <!-- <div class="divider"></div> -->
            <div class="number down">04</div>
         </div>
      </div>
   </div>
</template>

<style scoped>
#section-05 {
   width: 100%;
   height: 100%;
   background-image: url(../assets/BG_LP_fb.jpg);
   background-position: center;
   background-repeat: no-repeat;
   background-size: cover;
   border-radius: 0 0 50px 50px;
   display: flex;
   justify-content: center;
   align-items: center;
}
#section-05 .container {
   display: flex;
   align-items: center;
   justify-content: space-between;
   width: 100%;
   margin-top: 100px;
   margin-bottom: 100px;
   position: relative;
}

.arrow {
   width: 56px;
   height: 56px;
   background-color: #26C6D0;
   border-radius: 50%;
   border: 0;
   outline: 0;
   position: relative;
   cursor: pointer;
}
.arrow::before {
   content: '';
   position: absolute;
   left: 55%;
   top: 50%;
   width: 30%;
   height: 30%;
   border-left: 3px solid #fff;
   border-bottom: 3px solid #fff;
   transform: translate(-50%, -50%) rotate(45deg);
}

.right {
   transform: rotate(-180deg);
}
.view { 
   position: relative;
   width: 40%;
}

.view .pic {
   max-width: 540px;
   width: 100%;
   height: 100%;
   border-radius: 30px;
   overflow: hidden;
}
.view .btn {
   margin: 0;
   /* margin-left: 0;
   margin-right: 0;
   margin-top: 0; */
   padding: 40px 20px;
   position: absolute;
   bottom: -60px;
   right: -50px;
   /* left: 70%; */
}
.text {
   width: 40%;
   padding: 50px;
}
.text h5 {
   font-style: normal;
   font-weight: 700;
   font-size: 16px;
   line-height: 19px;
   letter-spacing: 2px;
   color: #FFFFFF;
   padding-bottom: 3%;
}
.text .title {
   margin: 0;
   color: #ffff;
   display: inline-block;
}
.text .title:before {
   bottom: 5px;
   left: -5px;
   right: -5px;
   background-color:#26C6D0;
   height: 5px;
}
.text p {
   color: #ffff;
   text-align: left;
   line-height: 24px;
   padding-top: 8%;
}

.page {
   width: 54px;
   height: 54px;
   position: absolute;
   top: 0;
   right: 0;
   /* background-color: red; */
   margin-right: 60px;
   z-index: 10;
   background:
    linear-gradient(-45deg, transparent 48.5%, #26C6D0 48.5%, #26C6D0 50%, transparent 50%);

}

/* .page::after {
   content: '';
   position: absolute;
   left: 0;
   right: 0;
   width: 100%;
   border-bottom: 3px solid #26C6D0;
} */

.page .number {
   color: #fff;
   font-style: normal;
   font-weight: 600;
   font-size: 16px;
   line-height: 19px;
   letter-spacing: 2px;
   position: absolute;
   cursor: pointer;
}

.page .number.down {
   bottom: 0;
   right: 0;
}
</style>
