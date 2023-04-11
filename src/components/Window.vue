<template>
<div class="container">
    <h1 class="titulo">* {{ titulo }}</h1>
    <div class="info">
        <img :src=imgPath alt="imagen">
        <p class="entrada">{{ texto }}
        </p>


    </div>
</div>
</template>

<script>

export default {
  name: "Window",
  props: {
    titulo: String,
    texto: String,
    imgPath: String,
  },
};
</script>
<style scoped>
.container{
    display: flex;
    flex-direction: column;
    justify-content: center;
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
    padding: 3vw;
    color: var(--text);
}
img{
    width: 200px;
    height: auto;
    margin-left: auto;
    margin-right: auto;
    margin-top: 2vw;
    border-radius: 250px;
}
.info{
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: var(--infoBack);
}
@media screen and (max-width: 1000px) {
    .container{
        margin-top: 5vw;
        margin-bottom: 16vw;
        width: 80%;
        
    }
    .titulo{
        font-size: 6vw;
    }
    .entrada{
        padding: 5vw;
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