<script>
import AppFooterIn from './AppFooterIn.vue'
export default {
  name: 'AppFooter',
  components:{
    AppFooterIn,
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
  
    }
  }
}
  
</script>


<template>
   
  <footer>


    <div class="bg-overlay">
        <section id="form-area">
            <div class="ms-container text-white d-flex align-content-center">
                <h1 class="px-3">Our news Letter </h1>
                <div class="box-text px-5 gap-2">
                        <label for="inputPassword6"><svg class="svg-msg svg-inline--fa fa-message" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="message" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M511.1 63.1v287.1c0 35.25-28.75 63.1-64 63.1h-144l-124.9 93.68c-7.875 5.75-19.12 .0497-19.12-9.7v-83.98h-96c-35.25 0-64-28.75-64-63.1V63.1c0-35.25 28.75-63.1 64-63.1h384C483.2 0 511.1 28.75 511.1 63.1z"></path></svg></label>
                            <div class="col-auto">
                                <input type="password" id="inputPassword6"  class="ms-form-control" aria-describedby="passwordHelpInline" placeholder="Enter Your Email">
                            </div>
                        <div class="box-send text-center">
                            Subscribe
                        </div>
                </div>
                
            </div>
        </section>
        <div class="ox-container">
            <nav class="navbar navbar-expand-lg">
                <div class="container">
                    <img src="../assets/img/menulogo.png" alt="">
                    <div class="link-group">
                        <ul class="navbar-nav me-auto mb-2 mb-lg-0 text-white gap-3">
                            <li v-for="(link, index) in links" :key="index" class="nav-item">
                                <a  :id="link.text + 'Dropdown'" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                                    {{ link.text }}
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </nav> 
        </div>
        
        
    <AppFooterIn></AppFooterIn>
    <AppSocialFooter></AppSocialFooter>
    </div>
  </footer>


</template>





<style scoped>


.container {
    border-bottom: grey 1px solid;
}

.ox-container {
    position: absolute;
    bottom: 30%;
    left: 0;
    width: 100%;
    height: 50px; /* Altezza desiderata del rettangolo rosso */
}

.card-body {
    background-color: transparent !important;
}
.card {
    background-color: transparent !important;
}

.red-rectangle {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 50px; /* Altezza desiderata del rettangolo rosso */
    background-color: red;
}

.ms-form-control {
    background-color: transparent;
    border: none;
}



.box-send {
    width: 100px;
    height: 25px;
    background-color: #00AC4D;
    color: #202046;
    font-weight: bolder;
    border-radius: 20px;
    margin-left: auto;

}

.box-text {
    margin-left: 300px;
    width: 600px;
    height: 50px;
    background-color: #191935;
    border-radius: 20px;
    padding-left: 10px;
    display: flex; 
    justify-content:start;
    align-items: center; 
}

.ms-container {
    margin: 0;
    width: 1240px;
    height: 150px;
    background-color:#202046;
    position: absolute;
    left: 17%;
    bottom: 375px;
    z-index:24;
    align-items: center;
    border-radius: 1%;
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

.svg-msg {
    width: 20px;
  height: 20px;
  color:#00AC4D;

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


.navbar-nav .nav-link {
  color: white;
}

footer {
  position: relative;
  background-image: url("../assets/img/footer-bg.png");
  height: 446px;
  width: 100%;
  background-size: 100% 100%;
}

.bg-overlay{
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 446px;
  background-color: rgba(19, 19, 35, 0.5);
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
