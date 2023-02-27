<script setup>
import HelloWorld from './components/dcHeader.vue'
import dcMain from './components/dcMain.vue'
import dcFooter from './components/dcFooter.vue'


</script>

<template>
  <HelloWorld />
  <dcMain />
  <dcFooter />
</template>

<style lang="scss" scoped>
@use "./assets/scss/general.scss";
@use "./assets/scss/font.scss";
</style>