




<template>
  <div class="container">
    <div class="page">
      <Header />
      <Banner />
      <Cards />
    </div>
  </div>

  <router-view />
</template>
<script>
import Banner from './components/Banner.vue';
import Cards from './components/Cards.vue';
import Header from './components/Header.vue';
export default {
  components: { Header, Banner, Cards }
}
</script>
<style lang="scss"></style>
