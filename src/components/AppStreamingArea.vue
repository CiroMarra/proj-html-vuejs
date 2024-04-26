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
                    <div class="col">
                        <div class="card mb-3">
                            <div class="card-body text-start">
                                <h6 class="ms-h6">Live Streaming</h6>
                                <h1 class="ms-h1 text-white">Checkout Our Live Streaming</h1>
                            </div>
                        </div>
                        <div class="col  ">
                            <div class="row">
                                <div class="col">
                                    <div class="card" style="width: 19rem;">
                                        <img src="../assets/img/b3.png" class="card-img-top" alt="...">
                                        <div class="card-body">
                                            <h5 class="card-title text-white">League of Legends</h5>
                                            <small class="text-white">Vestibulum ac diam sit amet quam vehicula</small>
                                        </div>    
                                    </div>
                                </div>
                                <div class="col">
                                    <div class="card" style="width: 19rem;">
                                        <img src="../assets/img/b3.png" class="card-img-top" alt="...">
                                        <div class="card-body">
                                            <h5 class="card-title text-white">League of Legends</h5>
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

.game-title {
    position: absolute;
    top: 58%;
    left: 503px;
    font-size: 30px;
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
    height: 40vw;
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