<script setup>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import SocialBar from './components/SocialBar.vue'
</script>

<template>
  <div>
    <Header />
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







</style>
