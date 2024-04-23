<script>
export default {
  name: 'AppMain',
  data() {
    return {
    };
  }
}
</script>

<template>
    <section class="ms-bg-section">
        <div class="container position-relative">
            <div class="box-img">
                <img src="../assets/img/1.png" alt="" class="mx-4 py-3 px-2">
                <img src="../assets/img/2.png" alt="" class="mx-4 py-3 px-2">
                <img src="../assets/img/3.png" alt="" class="mx-4 py-3 px-2">
                <img src="../assets/img/4.png" alt="" class="mx-4 py-3 px-2">
                <img src="../assets/img/5.png" alt="" class="mx-4 py-3 px-2">
                <img src="../assets/img/6.png" alt="" class="mx-4 py-3 px-2">
            </div>
        </div>
    </section>

</template>

<style>
 .ms-bg-section {
    background-color: #191935;
    height: 45vw;
    color: white;
 }

 .box-img {
    background-color: #202046;
    height: 200px;
    width: 1230px;
    position: absolute;
    bottom: -100px;
    left: 40px;

 }
</style>