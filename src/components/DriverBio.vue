<script setup>
  import { defineProps} from 'vue';

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
    },
    imgSrc: {
      type: String,
      required: true
    }
  })
</script>


<template>
  <div class="container-fluid bio-container">
    <div class="row justify-content-center">
      <div class="col-6 position-relative">
        <img class="bio-img" :src="props.imgSrc" alt="bio-pic" />
        <p class="overlay-name"><i>{{ props.firstName + " " + props.lastName }}</i></p>
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
  font-family: AudiType-ExtendedBold,Arial, Helvetica, sans-serif;
  color: #ffc11c;
  font-size: 1.5rem;
  background-color: gray;
  opacity: 70%;
  padding: 5px;
  border-radius: 5px;
}
</style>
