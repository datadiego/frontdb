<template>
    <div class="container">
        <p class="texto">This is the footer there's no more internet from here</p>

    </div>
</template>

<script>

</script>

<style scoped>
.container{
    background-color: black;
    color: white;
    position: absolute;
    bottom: 0;
    width: 100%;
    padding-bottom: 1rem;
    height: 2.5rem;
}
.texto{
    font-size: 1vw;
}
@media screen and (max-width: 1000px) {
    .texto{
        font-size: 3vw;
    }
}
</style>