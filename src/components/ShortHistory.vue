<template>
  <div id="short-history" class="container-fluid mt-5 mb-5" ref="audiHistory">
    <div class="row justify-content-center">
      <div class="col-9 text-center">
        <h1 class="quote"><i>"WRC is for boys, Group B was for men."</i> - Juha Kankkunen</h1>
      </div>
    </div>
    <div class="row mt-5 justify-content-center">
      <div class="col-4 center-it">
        <p>
          In the annals of automotive lore, there exists a tumultuous chapter that reverberates with
          the thunderous symphony of unbridled power and audacious speed—the era of Group B rally
          racing. Born in the early 1980s, Group B emerged as a crucible of automotive insanity,
          where manufacturers pushed the boundaries of performance to unprecedented heights. At the
          epicenter of this automotive maelstrom stood the legendary Audi Quattro, a machine that
          not only left an indelible mark on rallying but also reshaped the very essence of the
          sport.
        </p>
      </div>
      <div class="col-3 center-it">
        <div class="pic-con zoom-wrapper">
          <img class="pic" src="../assets/images/history-img.png" alt="old audi photo" />
        </div>
      </div>
    </div>
    <div class="row mt-5 justify-content-center">
      <div class="col-3 center-it">
        <div class="pic-con zoom-wrapper">
          <img class="pic" src="../assets/images/old-audi.jpg" alt="old audi mid corner photo" />
        </div>
      </div>
      <div class="col-4 center-it">
        <p>
          The Audi Quattro, with its revolutionary all-wheel-drive system, became the vanguard of a
          new era in rally racing. The conventional wisdom of rear-wheel-drive supremacy was
          shattered as the Quattro's distinctive five-cylinder turbocharged engine roared to life.
          Audi's audacious move not only defied tradition but propelled the Quattro to a dominant
          position on rally stages worldwide. The unmistakable growl of its powerplant, coupled with
          the relentless traction of quattro technology, transformed the Quattro into an unstoppable
          force, conquering gravel, mud, and snow with unparalleled ferocity. Yet, the glory of
          Group B was not without its perils. The pursuit of speed and power reached a fever pitch,
          culminating in tragic accidents that prompted the FIA to halt the madness in 1986. The
          curtain fell on Group B, ending an era that had redefined the limits of motorsport.
        </p>
      </div>
    </div>
    <div class="row mt-5 justify-content-center">
      <div class="col-4 center-it">
        <p>
          Nevertheless, the legacy of Group B endures as a testament to the uncompromising passion
          that fueled an era of automotive excess. The Audi Quattro, with its iconic design and
          pioneering technology, remains a symbol of innovation and courage. Though Group B may have
          been relegated to the archives of history, the spirit it embodied—the relentless pursuit
          of victory against all odds—continues to inspire automotive enthusiasts and rally
          aficionados alike. In the echoes of revving engines and rallying tales, the Audi Quattro
          stands as a timeless icon, a testament to an era when rally racing reached the zenith of
          exhilarating madness.
        </p>
      </div>
      <div class="col-3 center-it">
        <div class="pic-con zoom-wrapper">
          <img class="pic" src="../assets/images/group-b-lineup.jpg " alt="old audi photo" />
        </div>
      </div>
    </div>
  </div>
</template>

<script></script>

<style scoped>
.quote {
  font-family: AudiType-Light, Arial, Helvetica, sans-serif;
}
.pic {
  width: 100%;
  height: auto;
}
.pic-con {
  width: 27rem;
}
.center-it {
  display: flex;
  align-items: center;
  justify-content: center;
}
.zoom-wrapper {
  overflow: hidden;
  border-radius: 5%;
}

.zoom-wrapper img {
  object-fit: cover;
  transition: ease-out 0.3s;
}
.zoom-wrapper:hover img {
  transform: scale(1.2);
}
</style>
