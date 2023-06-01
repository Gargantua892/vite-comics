<script setup>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import ServiceBar from './components/ServiceBar.vue';
import SocialBar from './components/SocialBar.vue';
import ComicsList from './components/ComicsList.vue';
</script>

<template>
  <div>
    <Header />
    <main>
      <div class="jumbo">
      </div>
      <div class="container py-4">
        <ComicsList class="my-5" />
      </div>
      <ServiceBar />
    </main>
    <Footer />
    <SocialBar />
  </div>
</template>

<style lang="scss">
@use '../styles/partials/variables.scss' as *;
@use '../styles/general.scss' as *;

h2{
  color: $primary;
}

main{
  background-color: $black;
}

.jumbo{
  background: url('./assets/img/flash_hub_regBanner.avif'), linear-gradient(90deg,#2a0541,#5816bd);
  min-height: 300px;
  background-repeat: no-repeat, no-repeat;
  background-size: contain;
  background-position: 90%;
}

.button{
  text-transform: uppercase;
  padding: 8px 12px;
  display: inline-block;
  max-width: 30%;

  &.button-solid{
    background-color: $primary;
  }
}






</style>
