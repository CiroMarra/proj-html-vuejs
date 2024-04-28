<script>
export default {
  name: 'AppTestimonial',
  
  data() {
    return {
      games: [
    {
        title: "Cristiano Messi ",
        description: "CEO/Founder",
        image: "./src/assets/img/test1.png"
    },
    {
        title: "Sergio Naymer",
        description: "Programmer",
        image: "./src/assets/img/test2.png"
    },
    {
        title: "Antonela Roccuzzo",
        description: "Project Manager",
        image: "./src/assets/img/test3.png"
    },
    {
        title: "Lionel Ramos",
        description: "Game Designer",
        image: "./src/assets/img/test4.png"
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
                <p class="ms-h6">Testimonials</p>
                <h1 class="ms-h1">
                    What Our Client Say
                </h1>
                <div class="ns-circle"><svg class="svg-inline--fa fa-right-long" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="right-long" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M504.3 273.6l-112.1 104c-6.992 6.484-17.18 8.218-25.94 4.406c-8.758-3.812-14.42-12.45-14.42-21.1L351.9 288H32C14.33 288 .0002 273.7 .0002 255.1S14.33 224 32 224h319.9l0-72c0-9.547 5.66-18.19 14.42-22c8.754-3.809 18.95-2.075 25.94 4.41l112.1 104C514.6 247.9 514.6 264.1 504.3 273.6z"></path></svg></div>
                    <div class="ns-circle-r"><svg class="svg-inline--fa fa-arrow-left-long" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="arrow-left-long" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M9.375 233.4l128-128c12.5-12.5 32.75-12.5 45.25 0s12.5 32.75 0 45.25L109.3 224H480c17.69 0 32 14.31 32 32s-14.31 32-32 32H109.3l73.38 73.38c12.5 12.5 12.5 32.75 0 45.25c-12.49 12.49-32.74 12.51-45.25 0l-128-128C-3.125 266.1-3.125 245.9 9.375 233.4z"></path></svg></div>
                    <div class="col" v-for="(game, index) in games" :key="index">
                        <div class="card" style="position: relative;">
                                <div class="black-overlay">
                                    <div class="text">
                                        <div class="card" style="width: 18rem;">
                                            <div class="card-body">
                                                <h5 class="ms-title"><svg class="svg-inline--fa fa-quote-left" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="quote-left" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512" data-fa-i2svg=""><path fill="currentColor" d="M96 224C84.72 224 74.05 226.3 64 229.9V224c0-35.3 28.7-64 64-64c17.67 0 32-14.33 32-32S145.7 96 128 96C57.42 96 0 153.4 0 224v96c0 53.02 42.98 96 96 96s96-42.98 96-96S149 224 96 224zM352 224c-11.28 0-21.95 2.305-32 5.879V224c0-35.3 28.7-64 64-64c17.67 0 32-14.33 32-32s-14.33-32-32-32c-70.58 0-128 57.42-128 128v96c0 53.02 42.98 96 96 96s96-42.98 96-96S405 224 352 224z"></path></svg></h5>
                                                <p class="card-text">Donec sollicitudin molestie malesuada. Vestibulum ac diam sit amet quam vehicula elementum sed sit amet dui.
                                                    Cras ultricies ligula sed magna dictum porta.
                                                    Donec rutrum congue leo eget.</p>
                                                <p class="ms-card-text">Mohammadd Sala</p>
                                                <small>CEO/Founder</small>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <img :src="game.image" class="ms-card-img" alt="...">
                                    
                                </div>
                        </div>
                    </div>
                    
              </div>
        </div>
    </div>
        

   </section>
   
</template>

<style scoped>

.ms-title {
    width: 34px;
    color: #00ac4d;
}
.ms-card-text {
    color: #00ac4d;
    font-weight: bolder;
}

.text {
    display: none;
}


.black-overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(20, 20, 46, 0); 
}

.black-overlay:hover {
    background-color: rgba(20, 20, 46, 1); 
    width: 96%;
    z-index: 3;
}

.black-overlay:hover .text {
    display: block;
}

.col {
    padding: 0px !important;
}

.ms-card-img {
    height: 400px;
    width: 310px;
    background-color: transparent;
}



.svg-social {
    width: 25px;
}

.circle-container {
    position: absolute;
    bottom: 94px; 
    left: 50%;
    transform: translateX(-50%);
    text-align: center;
}

.box-social {
    width: 40px;
    height: 40px;
    border-radius: 50%;
    background-color: #333287; 
    line-height: 40px; 
    margin: 0 10px;
    display: none;
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
    left: 74%;
    bottom: 44%;
    font-size: 16px;
    z-index: 2;
}

.ns-circle-r {
    width: 40px; 
    height: 40px;
    background-color: #333287;
    border-radius: 50%; 
    margin-left: 4px;
    display: flex; 
    justify-content: center; 
    align-items: center; 
    position: absolute;
    left: 22%;
    bottom: 44%;
    font-size: 16px;
    color: white;
    z-index: 2;
}

.card {
    border: none;
    background-color: transparent;
    color: white;
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
    background-image: url(./src/assets/img/test-grouptwo.png),  url(./src/assets/img/test-group.png);
    background-color: #202046;
    height: 35vw;
    background-size: 50%, 30%; 
    background-position: bottom left, top right; 
    background-repeat: no-repeat; 
}

.bg-overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(20, 20, 46, 0.3);
    z-index: 2;
  }
</style>