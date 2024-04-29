<script>
import AppHero from './AppHero.vue'
export default {
  name: 'AppHeader',
  
  components:{
    AppHero
  },
  props:{
    links: Array
  },
  mounted ()
  {
    console.log(this.links)
  },

  
  data() {
    return {
      shops: [
    {
        title: "Sony PS5 White",
        price: "Quality: $254",
        image: "./src/assets/img/cart1.png"
    },
    {
        title: "A4 Tec Mouse",
        price: "Quality: $121",
        image: "./src/assets/img/cart2.png"
    },
    {
        title: "Gear VR Led ",
        price: "Quality: $514",
        image: "./src/assets/img/cart3.png"
    },
]
      
  
    }
  }
}
  
</script>


<template>
   
  <header>
    <div class="bg-overlay">
      <nav class="navbar navbar-expand-lg">
      <div class="container">
        <img src="../assets/img/menulogo.png" alt="">
        <div class="collapse navbar-collapse mx-5" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0 text-white">
            <li v-for="(link, index) in links" :key="index" class="nav-item">
              <a :class="[{'ms-home-color': link.text === 'HOME'}, {'nav-link': true}, {'dropdown-toggle': link.text === 'HOME' || link.text === 'SHOP' || link.text === 'BLOG' || link.text === 'PAGES'}]" :id="link.text + 'Dropdown'" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                {{ link.text }}
                <span v-if="link.text === 'PAGES' && link.submenu.length > 0" class="caret"></span>
              </a>
              <li class="nav-item dropdown"> 
                <ul class="dropdown-menu drop-color" v-if="link.text === 'PAGES' && link.submenu.length > 0" :aria-labelledby="link.text + 'Dropdown'">
                  <li v-for="(submenu, subIndex) in link.submenu" :key="subIndex">
                    <a class="dropdown-item" :href="submenu.link">{{ submenu.text }}</a>
                  </li>
                </ul>
              </li>
            </li>
          </ul>
          <div class="circle-box mx-2">
            <svg class="svg svg-inline--fa fa-magnifying-glass" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="magnifying-glass" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M500.3 443.7l-119.7-119.7c27.22-40.41 40.65-90.9 33.46-144.7C401.8 87.79 326.8 13.32 235.2 1.723C99.01-15.51-15.51 99.01 1.724 235.2c11.6 91.64 86.08 166.7 177.6 178.9c53.8 7.189 104.3-6.236 144.7-33.46l119.7 119.7c15.62 15.62 40.95 15.62 56.57 0C515.9 484.7 515.9 459.3 500.3 443.7zM79.1 208c0-70.58 57.42-128 128-128s128 57.42 128 128c0 70.58-57.42 128-128 128S79.1 278.6 79.1 208z"></path></svg>
          </div>
          <div class="circle-box mx-2">
            <div class="lcircle-box">0</div>
            <button class="ms-buttone" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasRight" aria-controls="offcanvasRight"><svg class="svg svg-inline--fa fa-bag-shopping" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="bag-shopping" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512" data-fa-i2svg=""><path fill="currentColor" d="M112 112C112 50.14 162.1 0 224 0C285.9 0 336 50.14 336 112V160H400C426.5 160 448 181.5 448 208V416C448 469 405 512 352 512H96C42.98 512 0 469 0 416V208C0 181.5 21.49 160 48 160H112V112zM160 160H288V112C288 76.65 259.3 48 224 48C188.7 48 160 76.65 160 112V160zM136 256C149.3 256 160 245.3 160 232C160 218.7 149.3 208 136 208C122.7 208 112 218.7 112 232C112 245.3 122.7 256 136 256zM312 208C298.7 208 288 218.7 288 232C288 245.3 298.7 256 312 256C325.3 256 336 245.3 336 232C336 218.7 325.3 208 312 208z"></path></svg></button>
          </div>
          
        </div>
        
      </div>
    </nav> 
                <div class="offcanvas offcanvas-end" tabindex="1" id="offcanvasRight" aria-labelledby="offcanvasRightLabel">
                  <div class="offcanvas-header">
                    <h5 class="offcanvas-title" id="offcanvasRightLabel">Offcanvas right</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>
                  </div>
                  <div class="offcanvas-body">
                    <div class="">
                      <div class="item" v-for="item in shops" :key="item.id">            
                        <div class="card mb-3">
                           <div class="row g-0">
                              <div class="col-md-4">
                                <img :src="item.image" class="test">
                              </div>
                              <div class="col-md-8">
                                <div class="card-body gap-1">
                                  <h5 class="card-title">{{ item.title }}</h5>
                                  <p class="card-text">{{ item.price }} <svg class="svg-canvas svg-inline--fa fa-xmark" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="xmark" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 320 512" data-fa-i2svg=""><path fill="currentColor" d="M310.6 361.4c12.5 12.5 12.5 32.75 0 45.25C304.4 412.9 296.2 416 288 416s-16.38-3.125-22.62-9.375L160 301.3L54.63 406.6C48.38 412.9 40.19 416 32 416S15.63 412.9 9.375 406.6c-12.5-12.5-12.5-32.75 0-45.25l105.4-105.4L9.375 150.6c-12.5-12.5-12.5-32.75 0-45.25s32.75-12.5 45.25 0L160 210.8l105.4-105.4c12.5-12.5 32.75-12.5 45.25 0s12.5 32.75 0 45.25l-105.4 105.4L310.6 361.4z"></path></svg></p>
                                </div>
                              </div>
                            </div>
                        </div>
                      </div>
                    </div>
                      <div class="total-price d-flex justify-content-between align-items-center">
                        <div class="order text-white">Total Order</div>
                        <div class="cost text-white">$854.00</div>
                      </div>
                    <div class="bottone d-flex justify-content-center align-items-center py-5">
                      <button class="ms-btn">CHECK OUT</button>
                    </div>
                    
                  </div>
                </div>
    
    <AppHero></AppHero>
    
    </div>
     
    
  </header>


</template>





<style scoped>

.cost {
  padding-right: 10px;
}

.ms-btn {
  background-color: #05CC7C;
  font-weight: bolder;
  color: #191935;
  width: 250px;
  height: 50px;
}

.svg-canvas {
  width: 11px;
  color: #05CC7C;

}

.card {
  background-color: transparent;
  border: none;
  color: white;
}


.offcanvas, .offcanvas-header {
  background-color: transparent;

}


.offcanvas-body, .offcanvas-header {
  background-color: rgba(20, 20, 46, 0.5)
}

.test {
  border: #05CC7C solid 1px;
  width: 100px;
  height: 80px;
}

.ms-buttone {
  border: none;
  background-color: transparent;
}

.circle-box {
  width: 40px;
  height: 40px;
  background-color: white;
  display: flex;
  justify-content: center; 
  align-items: center; 
  border-radius: 50%;
  position: relative;
}
.svg {
  width: 20px;
  height: 20px;
  color: #333287;
}

.lcircle-box {
  width: 25px;
  height: 25px;
  background-color: #4350FF;
  display: flex;
  justify-content: center; 
  border-radius: 50%;
  position: absolute;
  bottom: 20px;
  left: 31px;
  color: white;
}

li {
  list-style: none;
}
a {
  text-decoration: none;
}
.ms-home-color {
  color: #05CC7C !important;
}

.navbar-nav .nav-link {
  color: white;
}

header {
  position: relative;
  background-image: url("../assets/img/banner1.png");
  height: 45vw;
  width: 100%;
  background-size:cover;
  background-repeat: no-repeat;
}

.bg-overlay{
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 45vw;
  background-color: rgba(20, 20, 46, 0.5);
}

.drop-color {
  background-color: #202046;
}
.dropdown-item {
  color: #00AC4D;
}

.dropdown-menu:focus {
  color: white;
}
.navbar-nav .nav-link.show{
  color: white;
}
.navbar-nav {
  font-weight: bold;
}
</style>
