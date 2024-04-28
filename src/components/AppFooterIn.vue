<script>
import AppSocialFooter from './AppSocialFooter.vue'
export default {
  name: 'AppFooterIn',
  components:{
    AppSocialFooter,
  },
  props: {
    link: Object, 
  },

}
</script>

<template>
    <AppSocialFooter></AppSocialFooter>
</template>

<style scoped>
.circle-arrow {
  width: 38px;
  height: 38px;
  border-radius: 50%;
  justify-content: center; 
  align-items: center; 
  color: #191935;
}
.svg {
  width: 12px;
  color: #191935;
}
.card {
  background-color: transparent !important;
  border: none !important;
  color: white !important;
}

.ms-margin {
  margin-top: 220px;
}
 .ms-h6 {
  color: #00ac4d;
 }
 .ms-h1 {
  font-weight: 700;
  font-size: 60px;
  text-align: center;
 }

.ms-btn {
  background-color: #05cc7c !important;
  border: none;
  color: #191935;
  font-weight: bolder !important;
  text-align: center;
  margin: auto;

}
.ms-btn:hover {
  color: #191935 !important;

}
</style>