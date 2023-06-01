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







</style>
