<script>
export default {
  name: 'AppShop',
  data() {
    return {
      shops: [
    {
        title: "Asus Rog Strix A53",
        price: "$999.00",
        offer: "$970.00",
        image: "./src/assets/img/s1.png"
    },
    {
        title: "Asus Rog Strix A53",
        price: "$999.00",
        offer: "$970.00",
        image: "./src/assets/img/s2.png"
    },
    {
        title: "Asus Rog Strix A53",
        price: "$999.00",
        offer: "$970.00",
        image: "./src/assets/img/s3.png"
    },
    {
        title: "Asus Rog Strix A53",
        price: "$999.00",
        offer: "$970.00",
        image: "./src/assets/img/s4.png"
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
                <p class="ms-h6">Gamer Shop</p>
                <h1 class="ms-h1">
                    Explore Our Shop
                </h1>
                <div class="ns-circle"><svg class="svg-inline--fa fa-right-long" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="right-long" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M504.3 273.6l-112.1 104c-6.992 6.484-17.18 8.218-25.94 4.406c-8.758-3.812-14.42-12.45-14.42-21.1L351.9 288H32C14.33 288 .0002 273.7 .0002 255.1S14.33 224 32 224h319.9l0-72c0-9.547 5.66-18.19 14.42-22c8.754-3.809 18.95-2.075 25.94 4.41l112.1 104C514.6 247.9 514.6 264.1 504.3 273.6z"></path></svg></div>
                    <div class="ns-circle-r"><svg class="svg-inline--fa fa-arrow-left-long" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="arrow-left-long" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M9.375 233.4l128-128c12.5-12.5 32.75-12.5 45.25 0s12.5 32.75 0 45.25L109.3 224H480c17.69 0 32 14.31 32 32s-14.31 32-32 32H109.3l73.38 73.38c12.5 12.5 12.5 32.75 0 45.25c-12.49 12.49-32.74 12.51-45.25 0l-128-128C-3.125 266.1-3.125 245.9 9.375 233.4z"></path></svg></div>
                    <div class="col" v-for="(game, index) in shops" :key="index">
                        <div class="card" style="width: 18rem; position: relative;">
                            <img :src="game.image" class="ms-card-img-top" alt="...">
                            <div class="circle-container d-flex">
                                <div class="box-social">
                                    <svg class="svg-social svg-inline--fa fa-eye" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="eye" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512" data-fa-i2svg=""><path fill="currentColor" d="M279.6 160.4C282.4 160.1 285.2 160 288 160C341 160 384 202.1 384 256C384 309 341 352 288 352C234.1 352 192 309 192 256C192 253.2 192.1 250.4 192.4 247.6C201.7 252.1 212.5 256 224 256C259.3 256 288 227.3 288 192C288 180.5 284.1 169.7 279.6 160.4zM480.6 112.6C527.4 156 558.7 207.1 573.5 243.7C576.8 251.6 576.8 260.4 573.5 268.3C558.7 304 527.4 355.1 480.6 399.4C433.5 443.2 368.8 480 288 480C207.2 480 142.5 443.2 95.42 399.4C48.62 355.1 17.34 304 2.461 268.3C-.8205 260.4-.8205 251.6 2.461 243.7C17.34 207.1 48.62 156 95.42 112.6C142.5 68.84 207.2 32 288 32C368.8 32 433.5 68.84 480.6 112.6V112.6zM288 112C208.5 112 144 176.5 144 256C144 335.5 208.5 400 288 400C367.5 400 432 335.5 432 256C432 176.5 367.5 112 288 112z"></path></svg>
                                </div>
                                <div class="box-social">
                                    <svg class="svg-social svg-inline--fa fa-cart-flatbed" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="cart-flatbed" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 512" data-fa-i2svg=""><path fill="currentColor" d="M240 320h320c26.4 0 48-21.6 48-48v-192C608 53.6 586.4 32 560 32H448v128l-48-32L352 160V32H240C213.6 32 192 53.6 192 80v192C192 298.4 213.6 320 240 320zM608 384H128V64c0-35.2-28.8-64-64-64H31.1C14.4 0 0 14.4 0 32S14.4 64 31.1 64H48C56.84 64 64 71.16 64 80v335.1c0 17.6 14.4 32 32 32l66.92-.0009C161.1 453 160 458.4 160 464C160 490.5 181.5 512 208 512S256 490.5 256 464c0-5.641-1.13-10.97-2.917-16h197.9c-1.787 5.027-2.928 10.36-2.928 16C448 490.5 469.5 512 496 512c26.51 0 48.01-21.49 48.01-47.1c0-5.641-1.12-10.97-2.907-16l66.88 .0009C625.6 448 640 433.6 640 415.1C640 398.4 625.6 384 608 384z"></path></svg>
                                </div>
                                <div class="box-social">
                                    <svg class="svg-social svg-inline--fa fa-heart" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="heart" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M0 190.9V185.1C0 115.2 50.52 55.58 119.4 44.1C164.1 36.51 211.4 51.37 244 84.02L256 96L267.1 84.02C300.6 51.37 347 36.51 392.6 44.1C461.5 55.58 512 115.2 512 185.1V190.9C512 232.4 494.8 272.1 464.4 300.4L283.7 469.1C276.2 476.1 266.3 480 256 480C245.7 480 235.8 476.1 228.3 469.1L47.59 300.4C17.23 272.1 .0003 232.4 .0003 190.9L0 190.9z"></path></svg>
                                </div>
                            </div>
                        
                        </div>
                        <div class="card-body d-flex align-items-center justify-content-start py-3">
                                <div class="">
                                    <div class="star-gruop">
                                        <svg class=" svg-star-color svg-inline--fa fa-star-half-stroke text-white" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="star-half-stroke" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512" data-fa-i2svg=""><path fill="currentColor" d="M463.1 474.7C465.1 486.7 460.2 498.9 450.2 506C440.3 513.1 427.2 514 416.5 508.3L288.1 439.8L159.8 508.3C149 514 135.9 513.1 126 506C116.1 498.9 111.1 486.7 113.2 474.7L137.8 328.1L33.58 225.9C24.97 217.3 21.91 204.7 25.69 193.1C29.46 181.6 39.43 173.2 51.42 171.5L195 150.3L259.4 17.97C264.7 6.954 275.9-.0391 288.1-.0391C300.4-.0391 311.6 6.954 316.9 17.97L381.2 150.3L524.9 171.5C536.8 173.2 546.8 181.6 550.6 193.1C554.4 204.7 551.3 217.3 542.7 225.9L438.5 328.1L463.1 474.7zM288 376.4L288.1 376.3L399.7 435.9L378.4 309.6L469.2 219.8L343.8 201.4L288.1 86.85L288 87.14V376.4z"></path></svg>
                                        <svg class=" svg-star-color svg-inline--fa fa-star-half-stroke text-white" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="star-half-stroke" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512" data-fa-i2svg=""><path fill="currentColor" d="M463.1 474.7C465.1 486.7 460.2 498.9 450.2 506C440.3 513.1 427.2 514 416.5 508.3L288.1 439.8L159.8 508.3C149 514 135.9 513.1 126 506C116.1 498.9 111.1 486.7 113.2 474.7L137.8 328.1L33.58 225.9C24.97 217.3 21.91 204.7 25.69 193.1C29.46 181.6 39.43 173.2 51.42 171.5L195 150.3L259.4 17.97C264.7 6.954 275.9-.0391 288.1-.0391C300.4-.0391 311.6 6.954 316.9 17.97L381.2 150.3L524.9 171.5C536.8 173.2 546.8 181.6 550.6 193.1C554.4 204.7 551.3 217.3 542.7 225.9L438.5 328.1L463.1 474.7zM288 376.4L288.1 376.3L399.7 435.9L378.4 309.6L469.2 219.8L343.8 201.4L288.1 86.85L288 87.14V376.4z"></path></svg>
                                        <svg class=" svg-star svg-inline--fa fa-star-half-stroke text-white" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="star-half-stroke" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512" data-fa-i2svg=""><path fill="currentColor" d="M463.1 474.7C465.1 486.7 460.2 498.9 450.2 506C440.3 513.1 427.2 514 416.5 508.3L288.1 439.8L159.8 508.3C149 514 135.9 513.1 126 506C116.1 498.9 111.1 486.7 113.2 474.7L137.8 328.1L33.58 225.9C24.97 217.3 21.91 204.7 25.69 193.1C29.46 181.6 39.43 173.2 51.42 171.5L195 150.3L259.4 17.97C264.7 6.954 275.9-.0391 288.1-.0391C300.4-.0391 311.6 6.954 316.9 17.97L381.2 150.3L524.9 171.5C536.8 173.2 546.8 181.6 550.6 193.1C554.4 204.7 551.3 217.3 542.7 225.9L438.5 328.1L463.1 474.7zM288 376.4L288.1 376.3L399.7 435.9L378.4 309.6L469.2 219.8L343.8 201.4L288.1 86.85L288 87.14V376.4z"></path></svg>
                                        <svg class=" svg-star svg-inline--fa fa-star-half-stroke text-white" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="star-half-stroke" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512" data-fa-i2svg=""><path fill="currentColor" d="M463.1 474.7C465.1 486.7 460.2 498.9 450.2 506C440.3 513.1 427.2 514 416.5 508.3L288.1 439.8L159.8 508.3C149 514 135.9 513.1 126 506C116.1 498.9 111.1 486.7 113.2 474.7L137.8 328.1L33.58 225.9C24.97 217.3 21.91 204.7 25.69 193.1C29.46 181.6 39.43 173.2 51.42 171.5L195 150.3L259.4 17.97C264.7 6.954 275.9-.0391 288.1-.0391C300.4-.0391 311.6 6.954 316.9 17.97L381.2 150.3L524.9 171.5C536.8 173.2 546.8 181.6 550.6 193.1C554.4 204.7 551.3 217.3 542.7 225.9L438.5 328.1L463.1 474.7zM288 376.4L288.1 376.3L399.7 435.9L378.4 309.6L469.2 219.8L343.8 201.4L288.1 86.85L288 87.14V376.4z"></path></svg>
                                    </div>
                                    <h5 class="card-title">{{ game.title }}</h5>
                                    <p class="card-text">{{ game.description }}</p>
                                    <div class="d-flex gap-1">
                                        <p class="card-text ms-offer">{{ game.offer }}</p>
                                        <p class="card-text">{{ game.price }}</p>
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

.svg-star {
    width: 16px;
}

.svg-star-color{
    width: 16px;
    color: #00ac4d !important;

}

.ms-offer {
    color: #00ac4d;
}

.ms-card-img-top {
    max-width: 100%;
    max-height: 100%;
    margin: auto; 
    display: block;
}

.box-social:hover {
    background-color: #00ac4d;
}

.svg-social {
    width: 25px;
}

.circle-container {
    position: absolute;
    bottom: 40px; 
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

.card:hover .box-social {
    display: block;
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
    height: 300px;
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
    height: 33vw;
    background-image: url(./src/assets/img/shop-bg.png);
    background-size: 100% 100%;
}

.bg-overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(20, 20, 46, 0.7);
    z-index: 2;
  }
</style>