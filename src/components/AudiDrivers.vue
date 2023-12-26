<script setup>
import DriverBio from './DriverBio.vue'
import bios from '../../drivers.json'
import { ref, onMounted } from 'vue'

const driversInfo = ref([])

onMounted(() => {
  driversInfo.value = bios
})
</script>

<template>
  <div class="container-fluid">
    <div class="row text-center my-5">
      <div class="">
        <h2 class="noteable d-inline-block">Notable Drivers for Audi durring the Group B era</h2>
      </div>
    </div>
    <div class="row justify-content-center">
      <DriverBio
        v-for="driver in driversInfo"
        :key="driver.id"
        :shortBio="driver.bio"
        :firstName="driver.firstName"
        :lastName="driver.lastName"
        :imgSrc="driver.img"
        class="col-md-6 mb-4"
      />
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
  border-right: 2px solid;
  width: 100%;
  white-space: nowrap;
  overflow: hidden;
  animation:
    typing 5s steps(47),
    cursor 0.4s step-end infinite alternate;
}

/* cursor blinking */
@keyframes cursor {
  50% {
    border-color: transparent;
  }
}
/* typing */
@keyframes typing {
  from {
    width: 0;
  }
}
</style>
