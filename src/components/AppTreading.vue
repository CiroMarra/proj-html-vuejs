<script>
export default {
  name: 'AppTreading',
  data() {
    return {
      games: [
    {
        title: "Assasin's Creed",
        description: "Donec sollicitudin malesuada.",
        image: "./src/assets/img/protfolio1.png"
    },
    {
        title: "Call of Duty",
        description: "Donec sollicitudin malesuada.",
        image: "./src/assets/img/protfolio2.png"
    },
    {
        title: "Tomb Raiden",
        description: "Donec sollicitudin malesuada.",
        image: "./src/assets/img/protfolio3.png"
    },
    {
        title: "Mortal Combat X",
        description: "Donec sollicitudin malesuada.",
        image: "./src/assets/img/protfolio4.png"
    }
]
    }
  },
}
</script>

<template>
   <section class="ms-bg">
    <div class="bg-overlay">
    <div class="container text-white">
        <div class="container">
            <div class="row py-5">
                <p class="ms-h6">Treading Games</p>
                <h1 class="ms-h1">
                    Choose Who Is The Best in World!
                </h1>
                <div class="ns-circle"><svg class="svg-inline--fa fa-right-long" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="right-long" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M504.3 273.6l-112.1 104c-6.992 6.484-17.18 8.218-25.94 4.406c-8.758-3.812-14.42-12.45-14.42-21.1L351.9 288H32C14.33 288 .0002 273.7 .0002 255.1S14.33 224 32 224h319.9l0-72c0-9.547 5.66-18.19 14.42-22c8.754-3.809 18.95-2.075 25.94 4.41l112.1 104C514.6 247.9 514.6 264.1 504.3 273.6z"></path></svg></div>
                    <div class="ns-circle-r"><svg class="svg-inline--fa fa-arrow-left-long" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="arrow-left-long" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M9.375 233.4l128-128c12.5-12.5 32.75-12.5 45.25 0s12.5 32.75 0 45.25L109.3 224H480c17.69 0 32 14.31 32 32s-14.31 32-32 32H109.3l73.38 73.38c12.5 12.5 12.5 32.75 0 45.25c-12.49 12.49-32.74 12.51-45.25 0l-128-128C-3.125 266.1-3.125 245.9 9.375 233.4z"></path></svg></div>
                <div class="col" v-for="(game, index) in games" :key="index">
                    <div class="card" style="width: 18rem;">
                        <img :src="game.image" class="card-img-top" alt="...">
                        <div class="card-body d-flex align-items-center">
                            <div>
                                <h5 class="card-title">{{ game.title }}</h5>
                                <p class="card-text">{{ game.description }}</p>
                            </div>
                            <div class="circle">
                                <svg class="svg svg-inline--fa fa-play" aria-hidden="true" focusable="false"
                                    data-prefix="fas" data-icon="play" role="img" xmlns="http://www.w3.org/2000/svg"
                                    viewBox="0 0 384 512" data-fa-i2svg="">
                                    <path fill="currentColor"
                                        d="M361 215C375.3 223.8 384 239.3 384 256C384 272.7 375.3 288.2 361 296.1L73.03 472.1C58.21 482 39.66 482.4 24.52 473.9C9.377 465.4 0 449.4 0 432V80C0 62.64 9.377 46.63 24.52 38.13C39.66 29.64 58.21 29.99 73.03 39.04L361 215z">
                                    </path>
                                </svg>
                            </div>
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

.card:hover {
    background-color: #05CC75;
}

.card:hover .circle {
    background-color: #191935; 
}

.card:hover .svg {
    color: #00ac4d;
}

.svg  {
    width: 20px;
    height: 20px;
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
    background-image: url(./src/assets/img/protfolio-vector.png);
    background-size: 100% 100%;
}

.bg-overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(20, 20, 46, 0.5);
    z-index: 2;
  }
</style>