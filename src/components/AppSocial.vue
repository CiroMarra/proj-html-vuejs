<script>
import FacebookIcon from '../assets/img/facebook.svg';
import TwitterIcon from '../assets/img/twitter.svg';
import LinkedinIcon from '../assets/img/linkedin.svg';
import InstagramIcon from '../assets/img/instagram.svg';

export default {
  name: 'AppSocial',
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
  <div class="social position-relative d-flex flex-column mb-3">
    <div class="socials">
      <div v-for="social in socialIcons" :key="social.name" class="circle-social my-2 mx-5">
        <img :src="social.icon" :alt="social.name + ' Icon'" />
      </div>
    </div>
  </div>
</template>

<style>

.svg {
    color: white;
}

.circle-social img {
    filter: invert(100%);
    width: 30px;
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
    bottom: -10px;
    left: 90px;
}
</style>