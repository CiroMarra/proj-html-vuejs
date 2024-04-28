<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import './style/generic.sass';

export default {
  components: {
    AppHeader,
    AppMain, 
    AppFooter,
  },
  data() {
    return {

      links: [
        {
          id: 1,
          text: 'HOME',
          submenu: []
        },
        {
          id: 2,
          text: 'PAGES',
          submenu: [
            { text: 'About Us'},
            { text: 'Matches' },
            { text: 'Team' },
            { text: 'Squad' },
            { text: 'Squad Details' },
            { text: 'Comming Soon' },
            { text: '404' }
          ]
        },
        {
          id: 3,
          text: 'TOURNAMENT',
          submenu: []
        },
        {
          id: 4,
          text: 'SHOP',
          submenu: []
        },
        {
          id: 5,
          text: 'BLOG',
          submenu: []
        },
        {
          id: 6,
          text: 'CONTACT',
          submenu: []
        }
      ]
    };
  },
}
</script>


<template>
    <header>
      <!-- <ProductCard
        v-for="product in products"
        :key="product.id"
        :name="product.name"
        :price="product.price"
        :image="product.imageUrl"
      /> -->
    

      <AppHeader 
        :links="links"
      
      />
    </header>
    <main>
        <AppMain></AppMain>
    </main>
    <footer>
      <AppFooter :links="links"
      
      
      />
    </footer>
</template>

<style scoped>

</style>
