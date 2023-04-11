<script>
import Window from "../components/Window.vue";
import SignUp from "../components/SignUp.vue";
export default {
  name: "Home",
  components: {
    Window,
    SignUp
  },
  data(){
        return{

        }
  }
};
</script>

<template>
        <!-- <img class="logo" src="../assets/smiley.png" alt="logo" /> -->
        <SignUp />
</template>

<script>

</script>

<style scoped>
.logo{
        width: 10vw;
        height: auto;
        border: 6px solid black;
        border-radius: 200px;
        position: absolute;
        top: 10vh;
        left: 70vw;
        transform: rotate(20deg);

        background-color: yellow;
}
</style>