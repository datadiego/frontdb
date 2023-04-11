<script>
import Producto from "../components/Producto.vue";
import imagen1 from "../assets/imgs/gen (1).jpg";
import imagen2 from "../assets/imgs/gen (2).jpg";
import imagen3 from "../assets/imgs/gen (3).jpg";
import imagen4 from "../assets/imgs/gen (4).jpg";
import imagen5 from "../assets/imgs/gen (5).jpg";

export default {
    name: "Shop",
    components: {
        Producto,
    },
    methods: {
        onProductClick(product){
            this.selectedProduct = product;
            console.log(this.selectedProduct)
        }
    },
    data(){
        return{
            selectedProduct: null,
            aplicaciones : [
                {id: 1,title: "CoinApp", text: "Gestión, Wallet y consulta de compraventa de criptomonedas.", img: imagen1, tech:"Flask, Python, Javascript, HTML+CSS", link:"/projects/coinapp"},
                {id: 2, title: "Flash toki pona", text: "Aplicación de memorización de vocabulario en toki pona.", img: imagen2, tech:"Vuejs, Javascript, HTML+CSS", link:"/projects/flashcards"},
                {id: 5, title:"Twitter API Tools", text: "Utilidades para dessarrollo usando la API de twitter.", img: imagen3, tech: "Python, Tweepy", link:"/projects/twittertools"},
            ],

            arte : [
                {id: 1, title: "Ultrazone 0.2", text: "Coleccion NFT generativa en fxhash junto a @lxtxcx.", img: imagen4, tech:"p5js, JavaScript, fxhash", link:"/projects/ultrazone"},
                {id: 2, title: "Dithering", text: "Algoritmos de compresión y destrucción digital de imágenes.", img: imagen5, tech: "Python, PIL, OpenCV", link:"/projects/dithering"},
            ],
        }
    }
};


</script>

<template>
    <h1 class="titulo-seccion">Desarrollo web</h1>
    <div class="grid">
        <div v-for="producto in aplicaciones" @click="onProductClick(producto)" class="grid-item">
            <Producto :title="producto.title" :text="producto.text" :tech="producto.tech" :img=producto.img :link=producto.link />
        </div>
    </div>
    <h1 class="titulo-seccion">NetArt / Multimedia</h1>
    <div class="grid">
        <div v-for="producto in arte" @click="onProductClick(producto)" class="grid-item">
            <Producto :title="producto.title" :text="producto.text" :tech="producto.tech" :img=producto.img :link=producto.link />
        </div>
    </div>
</template>

<style scoped>

.grid{
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    justify-items: center;
    align-items: center;
    margin-top: 5vh;
    margin-bottom: 5vh;
    max-width: 80vw;
    margin-left: auto;
    margin-right: auto;
}
.titulo-seccion{
    text-align: center;
}
@media screen and (max-width: 1000px){
    .grid{
        display: grid;
        grid-template-columns: 1fr;
    }
    .titulo-seccion{
        font-size: 2rem;
        text-align: center;
    }
}
</style>