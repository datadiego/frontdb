<template>
    <div class="container">
        <h1 class="titulo">* Contactame</h1>
        <!-- <h2 class="introduccion">Lorem ipsum</h2> -->
        <div class="info">
            <img class="circle" src="../assets/img_2.jfif" alt="imagen">
            <p class="entrada">¡Gracias por tu visitarme! Si tienes alguna pregunta o comentario, no dudes en ponerte en contacto conmigo a través de correo electrónico. También puedes encontrarme en mis redes sociales.</p>
            <div class="redes">
                <a href="http://instagram.com"> <img class="icon" src="../assets/instagram.svg" alt=""></a>
                <a href="http://twitter.com"> <img class="icon" src="../assets/twitter.svg" alt=""></a>
                <a href="http://gmail.com"> <img class="icon" src="../assets/envelope.svg" alt=""></a>
                <a href="http://discord.com"> <img class="icon" src="../assets/discord.svg" alt=""></a>
            </div>

        </div>
    </div>
    </template>
    
    <script>
    
    export default {
      name: "Window",
    };
    </script>
    
    <style scoped>
    .container{
        display: flex;
        flex-direction: column;
        justify-content: center;
        width: 50vw;
        border: 3px solid black;
        border-radius: 16px;
        margin: 0 auto;
        box-shadow: 15px 15px black;
        margin-top: 1vw;
        margin-bottom: 10vh;
        
    }
    .titulo{
        font-size: 2.5vw;
        margin: 0;
        padding: 1vw;
        background-color: var(--titlesBack);
        color: var(--titlesFront);
        border-bottom: 3px solid black;

    }
    .introduccion{
        font-size: 3vw;
        margin: 0;
        padding: 2vw;
    }
    .entrada{
        font-size: 1.4vw;
        margin: 0;
        padding: 3vw;
        color: black;
    }
    .info{
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-evenly;
    }
    img{
        width: 200px;
        height: auto;
        margin-left: auto;
        margin-right: auto;
    }
    .circle{
        border-radius: 250px;
        margin-top: 2vw;
    }
    .redes img{
        width: 3vw;
        margin: 0;
        margin-right: 3vw;
        
    }
    
    .material-symbols-outlined{
        font-size: 100px;
    }
    .redes{
        display: flex;
        justify-content: center;
        margin-bottom: 1vw;
    }
    
    @media screen and (max-width: 1000px) {
        .container{
            margin-top: 5vw;
            width: 80%;
        }
        .titulo{
            font-size: 6vw;
        }
        .entrada{
            padding: 5vw;
            font-size: 3vw;
        }
        .introduccion{
            font-size: 5vw;
        }
        img{
            width: 30vw;
            height: auto;
            margin-left: auto;
            margin-right: auto;
        }
    img.icon{
        width: 10vw;
    }
    }
    </style>