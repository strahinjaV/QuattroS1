<script setup>
  import { defineProps, ref } from 'vue';

  const props = defineProps({
    firstName: {
      type: String,
    },
    lastName: {
      type: String,
    },
    shortBio: {
      type: String,
      required: true
    }
  })
</script>


<template>
  <div class="container-fluid bio-container">
    <div class="row justify-content-center">
      <div class="col-6 position-relative">
        <img class="bio-img" src="../assets/images/group-b-lineup.jpg" alt="bio-pic" />
        <p class="overlay-name">Sample Texxxxxxxxxxxxxxxxxxxxxxxxt</p>
      </div>
    </div>
    <div class="row justify-content-center">
      <div class="col-6">
        <p>{{ props.shortBio }}</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.bio-img {
  width: 100%;
  height: auto;
}
.center-it {
  display: flex;
  align-items: center;
  justify-content: center;
}
.overlay-name { 
  position: absolute;
  bottom: 2%;
  right: 7%;
  margin: 0;
}
</style>
