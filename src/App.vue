<script setup>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import ServiceBar from './components/ServiceBar.vue';
import SocialBar from './components/SocialBar.vue';
</script>

<template>
  <div>
    <Header />
    <main>
      <div class="container">
        <h2>Content goes here</h2>
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
  padding: 64px 0px 0px 0px;
  background-color: $black;
}







</style>
