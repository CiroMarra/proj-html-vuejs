<script>
import AppSocial from './AppSocial.vue'
export default {
  name: 'AppHero',
  components:{
    AppSocial,
  },
  props: {
    link: Object, 
  },

}
</script>

<template>
  <div class="container">
    <div class="card text-center d-flex justify-content-center ms-margin">
      <div class="card-body">
        <h6 class="ms-h6">WELCOME TO RAXG</h6>
        <h1 class="ms-h1">ARE YOU READY FOR YOUR NEXT CHALLENGE?</h1>
        <div class="d-flex justify-content-center">
          <a href="#" class="btn ms-btn mx-1">Go somewhere <svg class="svg svg-inline--fa fa-right-long" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="right-long" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M504.3 273.6l-112.1 104c-6.992 6.484-17.18 8.218-25.94 4.406c-8.758-3.812-14.42-12.45-14.42-21.1L351.9 288H32C14.33 288 .0002 273.7 .0002 255.1S14.33 224 32 224h319.9l0-72c0-9.547 5.66-18.19 14.42-22c8.754-3.809 18.95-2.075 25.94 4.41l112.1 104C514.6 247.9 514.6 264.1 504.3 273.6z"></path></svg></a>
          <a href="#" class="circle-arrow  ms-btn mx-1"><svg class=" circle-arrow svg svg-inline--fa fa-play" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="play" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512" data-fa-i2svg=""><path fill="currentColor" d="M361 215C375.3 223.8 384 239.3 384 256C384 272.7 375.3 288.2 361 296.1L73.03 472.1C58.21 482 39.66 482.4 24.52 473.9C9.377 465.4 0 449.4 0 432V80C0 62.64 9.377 46.63 24.52 38.13C39.66 29.64 58.21 29.99 73.03 39.04L361 215z"></path></svg></a>
        </div>
      </div>
    </div>
  </div>
<appSocial></appSocial>
</template>

<style scoped>
.circle-arrow {
  width: 38px;
  height: 38px;
  border-radius: 50%;
  justify-content: center; 
  align-items: center; 
  color: #191935;
}
.svg {
  width: 12px;
  color: #191935;
}
.card {
  background-color: transparent !important;
  border: none !important;
  color: white !important;
}

.ms-margin {
  margin-top: 220px;
}
 .ms-h6 {
  color: #00ac4d;
 }
 .ms-h1 {
  font-weight: 700;
  font-size: 60px;
  text-align: center;
 }

.ms-btn {
  background-color: #05cc7c !important;
  border: none;
  color: #191935;
  font-weight: bolder !important;
  text-align: center;
  margin: auto;

}
.ms-btn:hover {
  color: #191935 !important;

}
</style>
