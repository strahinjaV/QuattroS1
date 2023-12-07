<template> 
    <div class="container-fluid">
        <div class="row justify-content-center">
            <div class="col-md-6 text-center">
                    <div class="mask">
                        <video class="vid-con" src="../assets/Videos/audi-combined.mp4" autoplay muted loop></video>
                    </div>
            </div>
            <div class="col-md-4 center-it text-center">
                <h1 class="greeting-text text-break animate__animated animate__backInRight">Meet the Audi Quattro S1</h1>
            </div>
        </div>
    </div>
</template>

<script setup>

</script>

<style scoped> 

    .vid-con {
        width: 100%;
        height: auto;
    }
    .greeting-text {
        font-family: AudiType-Normal,Arial, Helvetica, sans-serif;
        font-size: 4vw;
        color: #2A2929;
    }
    .center-it {
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .mask {
        
    }
    
</style>