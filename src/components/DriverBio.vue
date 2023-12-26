<script setup>
import { defineProps } from 'vue'

const props = defineProps({
  firstName: {
    type: String
  },
  lastName: {
    type: String
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
          <p class="nameplate-name">
            <img class="nameplate-img" src="../assets/images/nameplate-asset.png" /><i>{{
              props.firstName + ' ' + props.lastName
            }}</i>
          </p>
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
  border-radius: 5%;
  height: auto;
}
.center-it {
  display: flex;
  align-items: center;
  justify-content: center;
}

.nameplate-name {
  position: absolute;
  bottom: 2%;
  right: 7%;
  margin: 0;
  font-family: AudiType-ExtendedBold, Arial, Helvetica, sans-serif;
  color: #ffc11c;
  font-size: 1.5rem;
  padding: 5px;
  border-radius: 5px;
  text-decoration: underline;
  background-color: rgba(0, 0, 0, 0.60);
}
.nameplate-img {
  width: 35px;
  margin-bottom: 3px;
}
.bio-con {
  background: hsla(45, 100%, 53%, 1);

background: linear-gradient(90deg, hsla(45, 100%, 53%, 1) 0%, hsla(0, 0%, 99%, 1) 100%);

background: -moz-linear-gradient(90deg, hsla(45, 100%, 53%, 1) 0%, hsla(0, 0%, 99%, 1) 100%);

background: -webkit-linear-gradient(90deg, hsla(45, 100%, 53%, 1) 0%, hsla(0, 0%, 99%, 1) 100%);

filter: progid: DXImageTransform.Microsoft.gradient( startColorstr="#ffc211", endColorstr="#FCFCFC", GradientType=1 );
}
</style>
