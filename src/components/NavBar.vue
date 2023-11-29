<template>
    <div class="wrapper">
        <nav class="navbar navbar-expand-lg custom">
            <div class="container-fluid">
                <img src="../assets/images/audi-rings.webp" alt="audi logo" class="navbar-img">
                <a class="navbar-brand p-0 m-2" href="#">Audi</a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse justify-content-center" id="navbarNavAltMarkup">
                    <div class="navbar-nav">
                        <a class="nav-link active" aria-current="page" href="#">Home</a>
                        <a class="nav-link" href="#">Features</a>
                        <a class="nav-link" href="#">Pricing</a>
                    </div>
                </div>
            </div>
        </nav>
    </div>
    
</template>

<style scoped>
    .wrapper {
        margin: 0;
        padding: 0;
        font-family: AudiType-Normal, Arial, Helvetica, sans-serif;
    }
    .custom {
        background-color: #ffc11c;
    }

    .navbar-img {
        width: 75px;
    }
</style>