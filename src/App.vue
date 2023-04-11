<script setup>
import Navbar from "./components/Navbar.vue";
import Header from "./components/Header.vue";
</script>

<template>
    <div id="page-container">
        <div id="content-wrap">
            <!-- <Header :text="'¡Bienvenido!'" /> -->
            <RouterView />
        </div>
            <Footer />
    </div>
</template>

<style scoped>
div{
    margin: 0;
    
}
#page-container {
    min-height: 100vh;
    position: relative;
    padding: 0;
    
}

#content-wrap {
    padding-bottom: 2.5rem;    /* Footer height */
}
</style>
