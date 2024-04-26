<template>
    <div class="card">
      <img :src="image" alt="Product Image" />
      <h3>{{ name }}</h3>
      <p>Price: ${{ price }}</p>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ProductCard',
    props: {
      name: String, 
      price: Number, 
      image: String, 
    },
    mounted() {
    console.log(this.name); 
    console.log(this.price); 
    console.log(this.image); 
  }
  };
  </script>
  
  <style scoped>
 
  </style>
  