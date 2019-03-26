<template>
    <div class="container-fluid">
        <div class="row">
            <header class="col-2">
                <figure class="text-center header-profile-container">
                    <img src="../assets/no-profile-image.png" class="header-img"/>
                    <p class="header-text">Nombre</p>
                    <p class="header-text">email@gmail.com</p>
                </figure>
                <div class="d-flex justify-content-around mb-lg-2">
                    <a href="#" class="header-text header-links">Iniciar Sesión</a>
                    <a href="#" class="header-text header-links">Registrarse</a>
                </div>

            </header>
        </div>
        <div class="row">
            <div class="col-2 aside-menu-container">
                <nav class="mt-lg-5">
                    <a href="url" class="aside-menu-item ">Inicio</a>
                    <a href="#pageSubmenu" data-toggle="collapse" aria-expanded="false"
                       class="dropdown-toggle aside-menu-item">Cursos</a>
                    <ul class="collapse list-unstyled ml-lg-4" id="pageSubmenu">
                        <li>
                            <a href="#" class="aside-menu-item">Programación</a>
                        </li>
                        <li>
                            <a href="#" class="aside-menu-item">UI</a>
                        </li>
                        <li>
                            <a href="#" class="aside-menu-item">UX</a>
                        </li>
                    </ul>
                    <a href="url" class="aside-menu-item">Sobre Nosotros</a>
                    <a href="url" class="aside-menu-item">Contacto</a>

                </nav>
            </div>
        </div>
        <div class="row">
            <footer class=" col-2">
                <div class="text-center">
                    <a href="url">
                        <img src="../assets/logotypes/linked-in-logo.svg" class="footer-links" alt="Linked-in">
                    </a>
                    <a href="url">
                        <img src="../assets/logotypes/twitter-logo.svg" class="footer-links" alt="Linked-in">
                    </a>
                    <a href="url">
                        <img src="../assets/logotypes/facebook-logo.svg" class="footer-links" alt="Linked-in">
                    </a>
                    <p class="footer-text">Copyright © 2019 by David Angulo</p>

                </div>
            </footer>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'AsideMenu',
        props: {
            msg: String
        }

    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    @import url('https://fonts.googleapis.com/css?family=Roboto:200,300,400,500,700');

    h1 {
        color: white;
        padding: 20px;
        text-align: center;
        font-family: 'Roboto', sans-serif;
    }

    .aside-menu-container {
        background-color: #aa00ff;
        height: 100vh;
        position: absolute;
    }

    .aside-menu-item {
        display: block;
        color: white;
        letter-spacing: 1px;
        padding: 20px;
        text-decoration: none;
        font-family: 'Roboto', sans-serif;
        font-weight: 300;
        border-radius: 5px;
    }

    .aside-menu-item:hover {
        background-color: #7200ca;
        box-shadow: 0 2px 7px 0 #7200ca;
        transition: 0.5s all;
    }

    .aside-menu-item:focus {
    }

    .share-logo {
        max-width: 100%;
        padding: 20px;
    }

    footer {
        position: fixed;
        bottom: 0;
        background-color: #e254ff;

    }

    header {
        background-color: #7200ca;
        width: 100%;
    }

    .footer-text {
        color: white;
        font-size: 10px;
        text-align: center;
        padding: 20px;
    }

    .header-text{
        color: white;
        font-family: 'Roboto', sans-serif;
        font-size: 14px;
        font-weight: 300;
        letter-spacing: 1px;

    }
    .header-img{
        max-width: 50%;
        max-height: 50%;
    }
    .header-profile-container{
        padding: 20px;
    }
    .header-links{
        padding: 20px;
        border-radius: 5px;
        margin-bottom: 10px;
        border: solid 1px white;
        text-decoration: none;

    }
    .header-links:hover{
        transition: 0.5s all;
        background-color: #e254ff;

    }
    .footer-links{
        margin-top: 20px;
        height: 60px;
        width: 60px;

    }

</style>
