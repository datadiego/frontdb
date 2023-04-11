<template>
    <div class="container">
        <nav>
          <ul>
            <li><router-link to="/">Home</router-link></li>
            <li><router-link to="/projects">Projects</router-link></li>
            <li><router-link to="/about">About</router-link></li>
          </ul>
        </nav>

    </div>
</template>

<script>

export default {
  name: "Navbar",
};
</script>

<style>
/* make elements from navbar always oneline */
.container {
  overflow: hidden;
  margin: 10px;
  display: flex;
  justify-content: center;
  width: 100%;
  
}

.container ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  margin-top: 1vw;
}

.container li {
  float: left;
  font-size: 1vw;
}

.container li a {
  color: var(--text);
  display: block;
  border: 2px solid var(--border);
  border-radius: 16px;
  margin: 2vw;
  margin-top: 0;
  box-shadow: 0 4px var(--shadow);
  text-align: center;
  padding: 8px 16px;
  text-decoration: none;
}

.container li a:hover {
  background-color: #F4F2F0;
}
@media screen and (max-width: 1000px) {
  .container{
    margin-bottom: 100px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }
  .container li {
    font-size: 4vw;
  }
  .container li a {
    margin-top: 3vw;
    padding: 2vw 4vw;
  }
  
}

</style>