<template>
        <router-link :to="link" >
    <div class="container">
            <img @click="$emit('click')" :src="img" alt="img" />
    </div>
    <div class="inferior">
        <h1 class="product-name">{{ title }}</h1>
        <p class="product-info">{{ text }}</p>
        <p class="tech-info">{{ tech }}</p>
    </div>
        </router-link>
</template>

<script>
export default {
    emits: ["click"],
    name: "Producto",
    props: {        
        title: String,
        text: String,
        tech: String,
        img: String,
        link: String,
    },
    };
</script>

<style scoped>
.container{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin: 0;
    
}
@keyframes moveGradient {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
}
.inferior{
    width: 20vw;
    margin: 0;
    padding: 0;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    color: black;
    border-bottom-left-radius: 20px;
    border-bottom-right-radius: 20px;
    margin-bottom: 3vh;
    background: white;
    
}
.product-name{
    margin: 0;
    padding: 0;
    font-size: 1.5rem;
}
.product-info{
    margin: 0;
    padding-left: 1vw;
    padding-right: 1vw;
    font-size: 1vw;
    text-align: center;
}
.tech-info{
    margin: 0;
    margin-bottom: 2vh;
    font-size: 0.8rem;
    text-align: center;
}
img{
    border-top-right-radius: 20px;
    border-top-left-radius: 20px;
    width: 20vw;
}
a{
    text-decoration: none;
    color: black;
}
@media screen and (max-width: 1000px){
    .container{
        margin: 0;
        padding: 0;
    }
    .inferior{
        width: 60vw;
        margin: 0;
        padding: 0;
        margin-bottom: 8vh;
        
    }
    .product-info{
        padding-top: 0;
        padding-left: 10vw;
        padding-right: 10vw;
    }
    img{
        width: 60vw;
    }
    .product-name{
        font-size: 1.2rem;
    }
    .product-info{
        font-size: 0.7rem;
    }    
}
</style>