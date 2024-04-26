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
      name: String, // Define prop type as String
      price: Number, // Define prop type as Number
      image: String,  // Define prop type as String
    },
    mounted() {
    console.log(this.name); // Log the 'name' prop
    console.log(this.price); // Log the 'price' prop
    console.log(this.image); // Log the 'image' prop
  }
  };
  </script>
  
  <style scoped>
  /* Styles for the product card */
  </style>
  