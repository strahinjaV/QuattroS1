<script setup>
  import NavBar from './components/NavBar.vue';
  import IntroVid from './components/IntroVid.vue';
  import History from './components/History.vue'
  import AudiDrivers from './components/AudiDrivers.vue'
  import 'animate.css'
</script>

<template>
  <div>
    <NavBar />
    <IntroVid />
    <History class="mb-5" />
    <AudiDrivers class="mt-5" />
  </div>
  
</template>

<style scoped>

</style>
