<script>
export default {
  name: 'AppMatch',
  data() {
    return {
        games: [
        {
        title: "Ninja Warrior Gaming",
        description: "Donec sollicitudin malesuada.",
        image: "./src/assets/img/m1.png"
    },
    {
        title: "Witch Gaming",
        image: "./src/assets/img/m2.png"
    },
    {
        title: "SkullG Gaming",
        image: "./src/assets/img/m3.png"
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
                    <p class="ms-h6">Treading Games</p>
                    <h1 class="ms-h1">
                        Choose Who Is The Best in World!
                    </h1>
                    <div class="ns-circle"><svg class="svg-inline--fa fa-right-long" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="right-long" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M504.3 273.6l-112.1 104c-6.992 6.484-17.18 8.218-25.94 4.406c-8.758-3.812-14.42-12.45-14.42-21.1L351.9 288H32C14.33 288 .0002 273.7 .0002 255.1S14.33 224 32 224h319.9l0-72c0-9.547 5.66-18.19 14.42-22c8.754-3.809 18.95-2.075 25.94 4.41l112.1 104C514.6 247.9 514.6 264.1 504.3 273.6z"></path></svg></div>
                        <div class="ns-circle-r"><svg class="svg-inline--fa fa-arrow-left-long" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="arrow-left-long" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M9.375 233.4l128-128c12.5-12.5 32.75-12.5 45.25 0s12.5 32.75 0 45.25L109.3 224H480c17.69 0 32 14.31 32 32s-14.31 32-32 32H109.3l73.38 73.38c12.5 12.5 12.5 32.75 0 45.25c-12.49 12.49-32.74 12.51-45.25 0l-128-128C-3.125 266.1-3.125 245.9 9.375 233.4z"></path></svg></div>
                    </div>


                    <div class="container text-center">
                        <div class="row">
                            <div class="col" v-for="(game, index) in games" :key="index">
                                <div class="card" style="width: 24rem;">
                                    <div class="d-flex justify-content-center align-items-center box-img ">
                                        <img :src="game.image" class="ms-card-img-top" alt="...">
                                    </div>
                                    <div class="card-body">
                                        <h5 class="card-title">{{ game.title }}</h5>
                                        <div class="d-flex justify-content-center">
                                            <div class="circle"><svg class="svg svg-inline--fa fa-youtube" aria-hidden="true" focusable="false" data-prefix="fab" data-icon="youtube" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512" data-fa-i2svg=""><path fill="currentColor" d="M549.7 124.1c-6.281-23.65-24.79-42.28-48.28-48.6C458.8 64 288 64 288 64S117.2 64 74.63 75.49c-23.5 6.322-42 24.95-48.28 48.6-11.41 42.87-11.41 132.3-11.41 132.3s0 89.44 11.41 132.3c6.281 23.65 24.79 41.5 48.28 47.82C117.2 448 288 448 288 448s170.8 0 213.4-11.49c23.5-6.321 42-24.17 48.28-47.82 11.41-42.87 11.41-132.3 11.41-132.3s0-89.44-11.41-132.3zm-317.5 213.5V175.2l142.7 81.21-142.7 81.2z"></path></svg></div>
                                            <div class="circle"><svg class="svg svg-inline--fa fa-message" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="message" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M511.1 63.1v287.1c0 35.25-28.75 63.1-64 63.1h-144l-124.9 93.68c-7.875 5.75-19.12 .0497-19.12-9.7v-83.98h-96c-35.25 0-64-28.75-64-63.1V63.1c0-35.25 28.75-63.1 64-63.1h384C483.2 0 511.1 28.75 511.1 63.1z"></path></svg></div>
                                        </div>
                                        <p class="card-text">9.45</p>
                                        <p class="card-text">1st November, 2022</p>
                                        <a href="#" class="btn ms-btn">View More</a>
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

.ms-card-img-top {
    width:  250px;
    height: 250px;
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
}






.svg  {
    width: 16px;
    height: 16px;
    color: #191935;
}

.circle {
    width: 40px; 
    height: 40px;
    background-color:#00ac4d;
    border-radius: 50%; 
    margin-left: 4px;
    display: flex; 
    justify-content: center; 
    align-items: center; 
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
    background-image: url(./src/assets/img/v-bg.png);
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