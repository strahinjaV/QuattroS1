<script setup>
import DriverBio from './DriverBio.vue'
import bios from '../../drivers.json'
import { ref, onMounted, provide } from 'vue'

const driversInfo = ref([])

onMounted(() => {
  driversInfo.value = bios

  
  targetElement.value = document.getElementById('audiHistory')
})


// Getting and providing the ref for the navbar 
const targetElement = ref(null)

provide('audiHistory',targetElement)
</script>

<template>
  <div class="container-fluid mt-5 backrd" ref="audiDrivers">
    <div class="row justify-content-center my-5">
      <div class="typewriter-con">
        <h2 id="drivers-part" class="noteable mt-3">Notable Drivers for Audi durring the Group B era</h2>
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
.backrd {
  background-color: black;
}

.typewriter-con { 
  display: inline-block;
  width: auto;
}
.noteable {
  font-family: AudiType-Light, Arial, Helvetica, sans-serif;
  font-size: 2.5rem;
  color: white;
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
