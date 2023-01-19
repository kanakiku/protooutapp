<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <div id="mycanvas">
          <canvas id="canvas" width="500" height="250"></canvas>
  </div>
  <br>
  <HelloWorld msg="Welcome to Your Vue.js App"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
//コードはここに書く？

}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
#mycanvas {
    width: 100%;
    max-width: 500px;
    margin: 40px auto;
    padding: 28px;
    border: 1px solid #ffffff;
    border-radius: 5px;
    background-color: transparent;
    box-shadow: 2px 2px 5px 0px rgba(200, 200, 200, 1);
    font-family: "Times New Roman";
}
</style>
