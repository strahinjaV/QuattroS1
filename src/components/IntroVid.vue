<template>
  <div id="in-video" class="container-fluid bg-black py-3">
    <div class="row justify-content-center">
      <div class="col-md-6 text-center position-relative">
        <div>
          <video
            id="intro-vid"
            class="vid-con"
            src="../assets/Videos/audi-combined.mp4"
            autoplay
            loop
            muted
          ></video>
          <div @click="toggleSound" class="sound-toggle">
            <i v-if="isMuted" class="fas fa-volume-mute"></i>
            <i v-else class="fas fa-volume-up"></i>
          </div>
        </div>
      </div>
      <div class="col-md-4 center-it text-center">
        <h1 class="greeting-text text-break animate__animated animate__fadeIn">
          Audi sets the challenge, Quattro sets the pace.
        </h1>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const isMuted = ref(true)

const toggleSound = () => {
  const video = document.getElementById('intro-vid')
  video.muted = !video.muted
  isMuted.value = video.muted
}

// Extending the fade in animation for the intro text (extended by 7x)
document.documentElement.style.setProperty('--animate-duration', '7s')
</script>

<style scoped>

.vid-con {
  width: 100%;
  height: auto;
  border-radius: 30px;
  position: relative;
}

.greeting-text {
  font-family: AudiType-Normal;
  font-size: 2.7vw;
  color: #ffc11c;
}

.center-it {
  display: flex;
  align-items: center;
  justify-content: center;
}

.sound-toggle {
  position: absolute;
  bottom: 20px;
  right: 40px;
  cursor: pointer;
  color: #ffc11c;
  font-size: 50px;
}
</style>
