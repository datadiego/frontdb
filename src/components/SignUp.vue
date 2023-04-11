<template>
    <div class="container">
        <h1 class="titulo">* Registro</h1>
        <div class="info">
            <div class="container-horizontal">
            <h2>Usuario:</h2>
            <input type="text" placeholder="Nombre de usuario" />
            </div>
            <div class="container-horizontal">
            <h2>Contraseña:</h2>
            <input type="password" placeholder="Contraseña" />
            
            </div>

            <div class="container-horizontal">       
            <h2>Confirmar contraseña:</h2>
            <input type="password" placeholder="Confirmar contraseña" />
            </div>
            <button>Registrarse</button>
        </div>
    </div>
    </template>
    
    <script>
    
    export default {
      name: "SignUp",
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
    .container-horizontal{
        display: flex;
        flex-direction: row;
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
    button{
        font: inherit;
        margin-top: 2vw;
        margin-bottom: 2vw;
        margin-left: auto;
        margin-right: auto;
        padding: 1vw;
        border-radius: 16px;
        background-color: var(--titlesBack);
        color: var(--titlesFront);
        font-size: 1.5vw;
        border: 3px solid var(--border);
        box-shadow: 5px 5px var(--shadow);
    }

    input {
        margin-top: 1vw;
        margin-bottom: 1vw;
        margin-left: 2vw;
        padding: 1vw;
        border-radius: 16px;
        background-color: var(--titlesBack);
        color: var(--titlesFront);
        font-size: 1.5vw;
        border: 3px solid var(--border);
        width: 100%;
        height: 2vh;
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