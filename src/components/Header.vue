<template>
    <div class="container">
    <h1>{{  text  }}</h1>
    </div>
</template>

<script>
export default {
  name: "Header",
  props: {
    text: String,
  },
};
</script>

<style scoped>

.container {
    overflow: hidden;
    display: flex;
    justify-content: center;
    width: 100%;
    margin-top: 2vw;
}

h1{
    border-top: 6px solid var(--border);
    border-bottom: 6px solid var(--border);
    font-size: 3vw;
    margin: 0;
    color: var(--text);

}

@media screen and (max-width: 980px) {
    .container{
        display: flex;
        justify-content: center;
        margin-top: 4vw;
        
    }
    h1{
        font-size: 10vw;
    }
}
</style>