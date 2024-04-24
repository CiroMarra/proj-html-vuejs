<script>
export default {
  name: 'AppGaming',
  data() {
    return {
    }
  },
}
</script>

<template>
    <section class="gaming-area position-relative">
      <div class="ms-bg-section-gaming-area"></div>
      <div class="bg-overlay d-flex justify-content-center align-items-center">
        <div class="container text-center text-white py-5">
          <div class="row">
                <div class="col">
                    <div class="card mb-3">
                            <div class="card-body text-start">
                                <h6 class="ms-h6">Our Extrem Feature</h6>
                                <h1 class="ms-h1">The Best Gaming Arena On The World!</h1>
                                <div class="card-text">
                                    Lorem ipsum dolor sit amet consectetur, adipisicing elit. Maiores id nisi, cum illum optio molestias mollitia iure accusantium repellat consequuntur, debitis, dolorem quisquam dolor unde nesciunt repellendus ad fuga. Ab?
                                </div>
                            </div>
                        </div>
                </div>
                    <div class="col">
                        <div class="row">
                            <div class="col-sm-6 mb-3 mb-sm-0 py-3">
                                <div class="card">
                                <div class="card-body ms-card-body ">
                                    <div class="ms-circle my-3">
                                        <img src="../assets/img/feature1.png" alt="" class="img-circle">
                                    </div>
                                    <h5 class="card-title">Live Streaming</h5>
                                    <p class="card-text">Nulla porttitor accumsan tincidunt.Pellentesque in.</p>
                                </div>
                                </div>
                            </div>
                            <div class="col-sm-6 mb-3 mb-sm-0 py-3">
                                <div class="card">
                                <div class="card-body ms-card-body-s">
                                    <div class="ms-circle my-3">
                                        <img src="../assets/img/feature2.png" alt="" class="img-circle">
                                    </div>
                                    <h5 class="card-title">Gaming News</h5>
                                    <p class="card-text">Nulla porttitor accumsan tincidunt.Pellentesque in.</p>
                                </div>
                                </div>
                            </div>
                            <div class="col-sm-6 mb-3 mb-sm-0 py-3">
                                <div class="card">
                                <div class="card-body ms-card-body-s">
                                    <div class="ms-circle my-3">
                                        <img src="../assets/img/feature3.png" alt="" class="img-circle">
                                    </div>
                                    <h5 class="card-title">Great Tournament</h5>
                                    <p class="card-text">Nulla porttitor accumsan tincidunt.Pellentesque in.</p>
                                </div>
                                </div>
                            </div>
                            <div class="col-sm-6 mb-3 mb-sm-0 py-3">
                                <div class="card">
                                <div class="card-body ms-card-body ">
                                    <div class="ms-circle my-3">
                                        <img src="../assets/img/feature4.png" alt="" class="img-circle">
                                    </div>
                                    <h5 class="card-title">Award Ceremony</h5>
                                    <p class="card-text">Nulla porttitor accumsan tincidunt.Pellentesque in.</p>
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

    .card-title {
        font-weight: bold;
        font-size: 30px;
    }

  .img-circle {
    width: 60px;
    height: 60px;
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
  .ms-circle {
    width: 100px;
    height: 100px;
    border-radius: 50%;
    background-color: #202046;
    display: flex;
    justify-content: center; 
     align-items: center; 
     margin: 0 auto;
  }
    .ms-h6 {
    color: #00ac4d;
    }
    .ms-h1 {
    font-weight: 700;
    font-size: 50px;
    text-align: start;
    }

    .ms-card-body {
        background-color: #05CC7C;
        border-radius: 5%;
        height: 300px;
        color:#191935;
        font-weight: bolder;
    }

    .ms-card-body-s {
        background-color: #333287;
        border-radius: 5%;
        height: 300px;
        color:white;
        font-weight: bolder;

    }
    .ms-card-body-s:hover {
        background-color: #05CC7C;
        color:#191935;
    }
    .ms-card-body:hover {
        background-color: #333287;
        color:white;
    }


   .card {
    background-color: transparent;
    color: white;
    border: none;
   } 
  .ms-bg-section-gaming-area {
    position: relative;
    background-color: #202046;
    height: 40vw;
    background-image: url(./src/assets/img/Vector.png);
  }
  </style>