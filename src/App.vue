<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import './style/generic.sass';

export default {
  components: {
    AppHeader,
    AppMain,
  }
}
</script>


<template>
    <header>
        <AppHeader></AppHeader>
    </header>
    <main>
        <AppMain></AppMain>
    </main>
</template>

<style scoped>
</style>
