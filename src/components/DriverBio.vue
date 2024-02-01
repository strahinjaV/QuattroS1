<script setup>

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
      <div class="col-6 position-relative zoom-wrapper">
        <img class="bio-img" :src="props.imgSrc" alt="bio-pic" />
        <p class="nameplate-name">
          <img class="nameplate-img" src="../assets/images/nameplate-asset.png" /><i>{{
            props.firstName + ' ' + props.lastName
          }}</i>
        </p>
      </div>
    </div>
    <div class="row justify-content-center">
      <div class="col-6 bio-text mt-3">
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
  background-color: rgba(0, 0, 0, 0.6);
}
.nameplate-img {
  width: 35px;
  margin-bottom: 3px;
}

.zoom-wrapper {
  overflow: hidden;
  border-radius: 5%;
}

.zoom-wrapper .bio-img {
  object-fit: cover;
  transition: ease-out 0.3s;
}
.zoom-wrapper .bio-img:hover {
  transform: scale(1.2);
  opacity: 90%;
}

.bio-text p {
  color: white;
  font-family: AudiType-Light, Arial, Helvetica, sans-serif;
  text-align: justify;
}
</style>
