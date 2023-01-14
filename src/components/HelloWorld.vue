<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      For a guide and recipes on how to configure / customize this project,<br>
      check out the
      <a href="https://cli.vuejs.org" target="_blank" rel="noopener">vue-cli documentation</a>.
    </p>
    <h3>Essential Links</h3>
    <ul>
      <li><a href="https://vuejs.org" target="_blank" rel="noopener">Core Docs</a></li>
      <li><a href="https://forum.vuejs.org" target="_blank" rel="noopener">Forum</a></li>
      <li><a href="https://chat.vuejs.org" target="_blank" rel="noopener">Community Chat</a></li>
      <li><a href="https://twitter.com/vuejs" target="_blank" rel="noopener">Twitter</a></li>
      <li><a href="https://news.vuejs.org" target="_blank" rel="noopener">News</a></li>
    </ul>
    <p>
      testtext
    </p>
      <p>count</p><input type="number" max="1000" min="10" :value="top" @change="bottom">
      <br>
      <div id="app">
          <canvas id="canvas" width="500" height="250"></canvas>
      </div>
      <!--<br>
      <p>分母</p><input type="number" max="1000" min="10" :value="bottom" @change="top">-->
      <br>
      <div class="relative">
        <img id="gazo" class="coffetree" src="https://drive.google.com/uc?export=view&id=1K2j0JCF9CppLWob6YvZYvJR-ROm0NEIJ" width="540" height="960">
        <img id = "beans1" src="https://drive.google.com/uc?export=view&id=1IR24pMQ6-A1cgiSEhIIR7p5TwPnqr5no" class="absolute">
      </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.relative {
  position: relative;
}
.absolute {
  position: absolute;
  right: 1000px;
  bottom: 1000px;
}
#app {
    width: 96%;
    max-width: 500px;
    margin: 40px auto;
    padding: 28px;
    border: 1px solid #ffffff;
    border-radius: 5px;
    background-color: transparent;
    box-shadow: 2px 2px 5px 0px rgba(200, 200, 200, 1);
    font-family: "Times New Roman";
}

#canvas {
    margin: 0 auto;
}

</style>
