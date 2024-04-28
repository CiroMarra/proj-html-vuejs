<script>
import FacebookIcon from '../assets/img/facebook.svg';
import TwitterIcon from '../assets/img/twitter.svg';
import LinkedinIcon from '../assets/img/linkedin.svg';
import InstagramIcon from '../assets/img/instagram.svg';

export default {
  name: 'AppSocialFooter',
  data() {
    return {
      socialIcons: [
        { name: 'Facebook', icon: FacebookIcon },
        { name: 'Twitter', icon: TwitterIcon },
        { name: 'Linkedin', icon: LinkedinIcon },
        { name: 'Instagram', icon: InstagramIcon }
      ]
    };
  }
}
</script>

<template>
     <div class="text d-flex gap-1">
        Copyright (c) RaxG | Designed by <div class="colore"> Ciro Marra</div> </div> 
    <div class="socials">
        <div v-for="social in socialIcons" :key="social.name" class="circle-social gap-5">
            <img :src="social.icon" :alt="social.name + ' Icon'" />
        </div>
    </div>
</template>

<style>
.colore {
    color: #05cc7c;
}
.text {
    color: white;
    position: absolute;
    left: 16%;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    bottom: 10px;
}

.svg {
    color: white;
}

.circle-social img {
    filter: invert(100%);
    width: 20px;
}


.circle-social {
    background-color: #202046;
    width: 50px;
    height: 50px;
    color: white;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: auto;
}

.circle-social:hover {
    background-color: #05cc7c;
}

.socials {
    color: white;
    position: absolute;
    left: 74%;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    bottom: 10px;
}
</style>