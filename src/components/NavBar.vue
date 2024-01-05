<template>
    <div class="wrapper">
        <nav class="navbar navbar-expand-lg custom">
            <div class="container-fluid bckg-custom sticky-top">
                <img src="../assets/images/audi-rings.webp" alt="audi logo" class="navbar-img">
                <a class="navbar-brand p-0 m-2" id="navbarCompany" href="#">Quattro</a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
                    <div class="navbar-nav">
                        <a class="nav-link changing-links ms-2" aria-current="page" href="#">Home</a>
                        <a class="nav-link changing-links ms-2" href="#">History</a>
                        <a class="nav-link changing-links ms-2" href="#">Drivers</a>
                    </div>
                </div>
            </div>
        </nav>
    </div>
    
</template>


<style scoped>
    .wrapper {
        font-family: AudiType-Normal, Arial, Helvetica, sans-serif;
        letter-spacing: 3px;
        box-shadow: 0px 5px 8px rgba(0, 0, 0, 0.25);
    }
    .custom {
        background-color: #ffc11c;
    }

    .navbar-img {
        width: 75px;
    }

    #navbarCompany {
        font-family: AudiType-Light;
        color: #2A2929;
    }

    /* Links animation  */
    a.changing-links {
        position: relative;
        text-decoration: none;
        font-family: AudiType-Light, Arial, Helvetica, sans-serif;
        padding: 0 10px;
        color: #2A2929
    }
    a.changing-links:after {
        content: "";
        position: absolute;
        background-color: #fff;
        height: 3px;
        width: 0;
        left:0;
        bottom: -10px;
        transition: 0.5s ease-in-out;
        font-family: AudiType-Normal;
    }
    a.changing-links:hover:after {
        width: 100%;
    }
    a.changing-links:hover {
        font-family: AudiType-Normal, Arial, Helvetica, sans-serif;
    }
    
</style>