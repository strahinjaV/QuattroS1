<script setup>
import DriverBio from './DriverBio.vue'
import bios from '../../../drivers.json'


</script>

<template>
  <div class="container-fluid">
    <div class="row text-center my-5">
      <h2 class="noteable">Notable Drivers for Audi durring the Group B era</h2>
    </div>
    <div class="row justify-content-center">
      <DriverBio v-for="i in 4" :key="i" class="col-md-6 mb-4" />
    </div>
  </div>
</template>

<style scoped>
.center-it {
  display: flex;
  align-items: center;
  justify-content: center;
}
.noteable {
  font-family: AudiType-Light, Arial, Helvetica, sans-serif;
  font-size: 2.5rem;
}
</style>
