<script>
export default {
  name: 'AppStreamingArea',
  data() {
    return {
    }
  },
}
</script>

<template>
    <section class="streaming-area position-relative">
        <div class="ms-bg-streaming"></div>
        <div class="bg-overlay d-flex justify-content-center align-items-center">
            <div class="container text-center">
                <div class="row ">
                    <div class="col">
                        <div class="card text-bg-dark">
                            <img src="../assets/img/v-1.png" class="card-img" alt="...">
                            <div class="card-img-overlay">
                                <div class="circle-play">
                                    <svg class="svg svg-inline--fa fa-play" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="play" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512" data-fa-i2svg=""><path fill="currentColor" d="M361 215C375.3 223.8 384 239.3 384 256C384 272.7 375.3 288.2 361 296.1L73.03 472.1C58.21 482 39.66 482.4 24.52 473.9C9.377 465.4 0 449.4 0 432V80C0 62.64 9.377 46.63 24.52 38.13C39.66 29.64 58.21 29.99 73.03 39.04L361 215z"></path></svg>
                                </div> 
                                
                            </div>
                         
                        </div>
                        <p class="game-title text-white">League of Legends</p> 
                    </div>
                    <div class="col position-relative">
                        <div class="card mb-3 ">
                            <div class="card-body text-start ms-position">
                                <h6 class="ms-h6">Live Streaming</h6>
                                <h1 class="ms-h1 text-white">Checkout Our Live Streaming</h1>
                            </div>
                        </div>  
                                <div class="bottonc d-flex">
                                    <div class="round-button"><svg class="svg-b svg-inline--fa fa-arrow-left-long" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="arrow-left-long" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M9.375 233.4l128-128c12.5-12.5 32.75-12.5 45.25 0s12.5 32.75 0 45.25L109.3 224H480c17.69 0 32 14.31 32 32s-14.31 32-32 32H109.3l73.38 73.38c12.5 12.5 12.5 32.75 0 45.25c-12.49 12.49-32.74 12.51-45.25 0l-128-128C-3.125 266.1-3.125 245.9 9.375 233.4z"></path></svg></div>
                                    <div class="round-button-r"><svg class="svg-b svg-inline--fa fa-right-long" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="right-long" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M504.3 273.6l-112.1 104c-6.992 6.484-17.18 8.218-25.94 4.406c-8.758-3.812-14.42-12.45-14.42-21.1L351.9 288H32C14.33 288 .0002 273.7 .0002 255.1S14.33 224 32 224h319.9l0-72c0-9.547 5.66-18.19 14.42-22c8.754-3.809 18.95-2.075 25.94 4.41l112.1 104C514.6 247.9 514.6 264.1 504.3 273.6z"></path></svg></div>
                                </div>
                                 
                        <div class="col position-relative ">
                            <div class="row ms-position-box">
                                <div class="col position-relative">
                                    <div class="card" style="width: 19rem;">
                                        <img src="../assets/img/v-small1.png" class="card-img-top" alt="...">
                                        <div class="card-body">
                                            <h5 class="card-title text-white">League of Legends</h5>
                                            <small class="text-white">Vestibulum ac diam sit amet quam vehicula</small>
                                        </div>    
                                    </div>
                                </div>
                                <div class="col ms-botton">
                                    <div class="card" style="width: 19rem;">
                                        <img src="../assets/img/v-small2.png" class="card-img-top" alt="...">
                                        <div class="card-body">
                                            <h5 class="card-title text-white">Doom</h5>
                                            <small class="text-white">Vestibulum ac diam sit amet quam vehicula</small>
                                        </div>    
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

.svg-b {
    width: 16px;
}

.bottonc {
    position: absolute;
    top: 120px;
    left: 80%;
}


.round-button {
    width: 40px;
    height: 40px;
    background-color: #ffffff;
    border-radius: 50%; 
    margin: 10px;
    display: flex;
    justify-content: center; 
     align-items: center;
}

.round-button-r {
    background-color: #00ac4d;
    color: white;
    width: 40px;
    height: 40px;
    border-radius: 50%; 
    margin: 10px;
    display: flex;
    justify-content: center; 
     align-items: center; 

}


.ms-position-box {
    position: absolute;
    top: 170px;
}

.ms-position {
    position: absolute;
    bottom: -140px
}

.game-title {
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0 auto;
    position: absolute;
    top: 62%;
    left: 36%;
    transform: translate(-59%, -50%);
    font-size: 36px;
}

small {
    font-size: 12px;
}


.card {
    background-color: transparent;
    border: none;
}
.ms-h6 {
    color: #00ac4d;
    }

    .ms-h1 {
    font-weight: 700;
    font-size: 45px;
    text-align: start;
    }

.svg {
    width: 40px;
    height: 40px;
}
.circle-play {
    width: 100px;
    height: 100px;
    border-radius: 50%;
    background-color: #00AC4D;
    display: flex;
    justify-content: center; 
     align-items: center; 
     margin: 0 auto;
     position: absolute;
     top: 50%;
     left: 50%;
    transform: translate(-50%, -50%);
}


.ms-bg-streaming {
    background-image: url(../assets/img/v-bg.png);
    height: 35vw;
    background-size: cover;
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