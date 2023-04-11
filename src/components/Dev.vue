<template>
    <div class="container">
        <h1 class="titulo">* Desarrollo Web</h1>
        <div class="info">
            <img src="../assets/img_2.jfif" alt="imagen">
            
            <h2>Lenguajes:</h2>
            <p class="entrada">
            * HTML+CSS+JavaScript                
            </p>
            <p class="entrada">
            Librerias: p5js, Threejs, Vuejs, Bootstrap, jQuery   
            </p>
            <p class="entrada">
            * Python
            </p>
            <p class="entrada">
            Librerias: Flask, APIFlask, requests, dotenv, matplotlib, opencv, tkinter, imageio
            </p>
            <p class="entrada">
            * Java
            </p>
            <p class="entrada">
            Librerias: Processing
            </p>
            <h2>Tecnologías:</h2>
            <p class="entrada">
            * Repositorios: Git, Github
            </p>
            <p class="entrada">
            * Frameworks: Flask, Vuejs, Bootstrap, jQuery
            </p>
            <p class="entrada">
            * Bases de datos: SQLite, MySQL
            </p>
            <p class="entrada">
            * Servicios: fxhash, Neocities, Netlify, Firebase
            </p>
            <h3>
                Puedes ver mis proyectos y mi repositorio.
            </h3>
    
    
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
        width: 50vw;
        border: 3px solid var(--border);
        border-radius: 16px;
        margin: 0 auto;
        box-shadow: 15px 15px var(--shadow);
        margin-top: 1vw;
        margin-bottom: 5vw;
    }
    .titulo{
        font-size: 2.5vw;
        margin: 0;
        padding:1vw;
        background-color: var(--titlesBack);
        color: var(--titlesFront);
        border-bottom: 3px solid var(--border);
    }
    .entrada{
        font-size: 1.4vw;
        margin: 0;
        color: var(--text);
    }
    img{
        width: 200px;
        height: auto;
        margin-left: auto;
        margin-right: auto;
        border-radius: 250px;
    }
    .info{
        display: flex;
        flex-direction: column;
        padding: 4vw;
        padding-top: 2vw;
        color: var(--text);
        background-color: var(--infoBack);
    }
ul{
    margin-top: 3vh;
    margin-bottom: 3vh;
    padding: 0;
    list-style-type: disc;
    list-style: circle;
    display: flex;
    flex-direction: column;
}
li{
    margin-left: 2vw;
    line-height: 0.1vw;
}
    @media screen and (max-width: 1000px) {
        h2{
            margin: 0;
            margin-bottom: 1vw;
            margin-top: 1vw;
        }
       
        .container{
            margin-top: 5vw;
            margin-bottom: 16vw;
            width: 80%;
            
        }
        .titulo{
            font-size: 6vw;
        }
        .entrada{
            font-size: 3vw;
        }
    
        img{
            width: 30vw;
            height: auto;
            margin-left: auto;
            margin-right: auto;
        }

    }
    </style>