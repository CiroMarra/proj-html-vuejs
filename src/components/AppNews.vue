<script>
export default {
  name: 'AppNews',
  data() {
    return {
        games: [
        {
        title: "Ninja Warrior Gaming",
        image: "./src/assets/img/b1.png"
    },
    {
        title: "Ghost Rider  Return",
        image: "./src/assets/img/b2.png"
    },
    {
        title: "League Of Legends",
        image: "./src/assets/img/b3.png"
    },
    {
        title: "Cyber Punk 2077",
        image: "./src/assets/img/b4.png"
    },
]
    }
  },
}
</script>

<template>
   <section class="ms-bg text-white">
    
    <div class="bg-overlay text-white">
                <div class="container">

                <div class="row py-5">
                    <p class="ms-h6">Latest News</p>
                    <h1 class="ms-h1">
                        Stay Updated With our Latest News Articles
                    </h1>
                    <div class="ns-circle"><svg class="svg-inline--fa fa-right-long" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="right-long" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M504.3 273.6l-112.1 104c-6.992 6.484-17.18 8.218-25.94 4.406c-8.758-3.812-14.42-12.45-14.42-21.1L351.9 288H32C14.33 288 .0002 273.7 .0002 255.1S14.33 224 32 224h319.9l0-72c0-9.547 5.66-18.19 14.42-22c8.754-3.809 18.95-2.075 25.94 4.41l112.1 104C514.6 247.9 514.6 264.1 504.3 273.6z"></path></svg></div>
                        <div class="ns-circle-r"><svg class="svg-inline--fa fa-arrow-left-long" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="arrow-left-long" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M9.375 233.4l128-128c12.5-12.5 32.75-12.5 45.25 0s12.5 32.75 0 45.25L109.3 224H480c17.69 0 32 14.31 32 32s-14.31 32-32 32H109.3l73.38 73.38c12.5 12.5 12.5 32.75 0 45.25c-12.49 12.49-32.74 12.51-45.25 0l-128-128C-3.125 266.1-3.125 245.9 9.375 233.4z"></path></svg></div>
                    </div>


                    <div class="container text-center">
                        <div class="row">
                            <div class="col" v-for="(game, index) in games" :key="index">
                                <div class="card" style="width: 18rem;">
                                    <img :src="game.image" class="ms-card-img-top" alt="...">
                                    <div class="card-body">
                                        <h5 class="card-title">{{ game.title }}</h5>
                                        <div class="d-flex justify-content-center gap-1 py-3">
                                         <div class="icon"><svg class="icon svg-icon svg-inline--fa fa-youtube" aria-hidden="true" focusable="false" data-prefix="fab" data-icon="youtube" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512" data-fa-i2svg=""><path fill="currentColor" d="M549.7 124.1c-6.281-23.65-24.79-42.28-48.28-48.6C458.8 64 288 64 288 64S117.2 64 74.63 75.49c-23.5 6.322-42 24.95-48.28 48.6-11.41 42.87-11.41 132.3-11.41 132.3s0 89.44 11.41 132.3c6.281 23.65 24.79 41.5 48.28 47.82C117.2 448 288 448 288 448s170.8 0 213.4-11.49c23.5-6.321 42-24.17 48.28-47.82 11.41-42.87 11.41-132.3 11.41-132.3s0-89.44-11.41-132.3zm-317.5 213.5V175.2l142.7 81.21-142.7 81.2z"></path></svg></div>
                                            <div class="card-text">By Admin</div>
                                            <div class="card-text">|</div>
                                           <div class="icon"><svg class="svg-icon  svg-inline--fa fa-calendar-days" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="calendar-days" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512" data-fa-i2svg=""><path fill="currentColor" d="M160 32V64H288V32C288 14.33 302.3 0 320 0C337.7 0 352 14.33 352 32V64H400C426.5 64 448 85.49 448 112V160H0V112C0 85.49 21.49 64 48 64H96V32C96 14.33 110.3 0 128 0C145.7 0 160 14.33 160 32zM0 192H448V464C448 490.5 426.5 512 400 512H48C21.49 512 0 490.5 0 464V192zM64 304C64 312.8 71.16 320 80 320H112C120.8 320 128 312.8 128 304V272C128 263.2 120.8 256 112 256H80C71.16 256 64 263.2 64 272V304zM192 304C192 312.8 199.2 320 208 320H240C248.8 320 256 312.8 256 304V272C256 263.2 248.8 256 240 256H208C199.2 256 192 263.2 192 272V304zM336 256C327.2 256 320 263.2 320 272V304C320 312.8 327.2 320 336 320H368C376.8 320 384 312.8 384 304V272C384 263.2 376.8 256 368 256H336zM64 432C64 440.8 71.16 448 80 448H112C120.8 448 128 440.8 128 432V400C128 391.2 120.8 384 112 384H80C71.16 384 64 391.2 64 400V432zM208 384C199.2 384 192 391.2 192 400V432C192 440.8 199.2 448 208 448H240C248.8 448 256 440.8 256 432V400C256 391.2 248.8 384 240 384H208zM320 432C320 440.8 327.2 448 336 448H368C376.8 448 384 440.8 384 432V400C384 391.2 376.8 384 368 384H336C327.2 384 320 391.2 320 400V432z"></path></svg></div>
                                            
                                           <div class="card-text">octomber 25, 2022</div>
                                        </div>
                                        <a href="#" class="btn ms-btn my-3">View More</a>
                                    </div>
                                </div>
                            </div>    
                        </div>
                    </div>
        </div>
    </div>
  
      

   </section>
   
</template>

<style scoped>


.ms-btn {
    background-color: #00ac4d;
    color: #191935;
    font-weight: bold;
}

.ms-btn:hover {
    background-color: none;
    color: #00ac4d;
    border: #00ac4d solid 1px;
}

.box-img {
    margin: 20px;
    width: 90%; 
    height: 300px; 
    background-color: #191935;
    margin-top: 20px;
    border-radius: 10%;
    
}



.ns-circle {
    width: 40px; 
    height: 40px;
    background-color:#00ac4d;
    border-radius: 50%; 
    margin-left: 4px;
    display: flex; 
    justify-content: center; 
    align-items: center; 
    position: absolute;
    left: 80%;
    bottom: 82%;
    font-size: 16px;
}

.ns-circle-r {
    width: 40px; 
    height: 40px;
    background-color:white;
    border-radius: 50%; 
    margin-left: 4px;
    display: flex; 
    justify-content: center; 
    align-items: center; 
    position: absolute;
    left: 77%;
    bottom: 82%;
    font-size: 16px;
    color: #191935;
}

.card {
    border: none;
    background-color: #202046;
    color: white;
    border-radius: 5%;
}


.svg-icon  {
    width: 16px;
    height: 16px;
    color: #00ac4d;
}



.svg  {
    width: 16px;
    height: 16px;
    color: #191935;
}


.ms-h6 {
    color: #00ac4d;
    }

    .ms-h1 {
    font-weight: 700;
    font-size: 45px;
    text-align: start;
    }

.ms-bg {
    position: relative;
    background-color: #202046;
    height: 40vw;
    background-size: 100% 100%;
}

.bg-overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(20, 20, 46, 0.8);
    z-index: 2;
  }
</style>