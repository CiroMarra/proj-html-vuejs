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
              1 of 2
            </div>
            <div class="col">
              2 of 2
            </div>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <style scoped>
  .bg-overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(20, 20, 46, 0.5);
    z-index: 2;
  }
  
  .ms-bg-section-gaming-area {
    position: relative;
    background-color: #202046;
    height: 40vw;
    background-image: url(./src/assets/img/Vector.png);
  }
  </style>