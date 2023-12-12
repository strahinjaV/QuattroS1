<script setup> 
    import DriverBio from './DriverBio.vue';
</script>

<template> 
    <div class="container-fluid">
        <div class="row justify-content-center">
                <DriverBio v-for="i in 4" :key="i" class="col-md-6 mb-4"  />
        </div>
    </div>
</template>

<style scoped>
    .center-it {
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>