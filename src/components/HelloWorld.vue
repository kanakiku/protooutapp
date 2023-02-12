<template>
      <p>count</p><input type="number" max="1000" min="10" :value="top" @change="bottom">
      <br>
      <!--<p>分母</p><input type="number" max="1000" min="10" :value="bottom" @change="top">-->
      <div class="relative">
        <img id="gazo" src="https://drive.google.com/uc?export=view&id=1K2j0JCF9CppLWob6YvZYvJR-ROm0NEIJ" width="540" height="960">
        <img id = "beans1" class="beans1" src="https://drive.google.com/uc?export=view&id=1IR24pMQ6-A1cgiSEhIIR7p5TwPnqr5no" >
        <img id = "beans2" class="beans2" src="https://drive.google.com/uc?export=view&id=1IR24pMQ6-A1cgiSEhIIR7p5TwPnqr5no" >
        <img id = "beans3" class="beans3" src="https://drive.google.com/uc?export=view&id=1IR24pMQ6-A1cgiSEhIIR7p5TwPnqr5no" >
        <img id = "beans4" class="beans4" src="https://drive.google.com/uc?export=view&id=1IR24pMQ6-A1cgiSEhIIR7p5TwPnqr5no" >
        <img id = "beans5" class="beans5" src="https://drive.google.com/uc?export=view&id=1IR24pMQ6-A1cgiSEhIIR7p5TwPnqr5no" >
        <img id = "beans6" class="beans6" src="https://drive.google.com/uc?export=view&id=1IR24pMQ6-A1cgiSEhIIR7p5TwPnqr5no" >
        <img id = "beans7" class="beans7" src="https://drive.google.com/uc?export=view&id=1IR24pMQ6-A1cgiSEhIIR7p5TwPnqr5no" >

      </div>
      <br>
      <!--ループサンプル
      <div v-for="fruit in fruits" :key="fruit">
        {{ fruit }}
      </div>
      -->
      <li v-for="image in images" :key="image.index">
      <img :src="image.src" alt="">
      </li>
      <br>
      
      <image v-for="n in 5" :key="n">{{ "image2.src" }}</image>

</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
  },
  /*
  data: () => {
    return {
      fruits: ["みかん", "りんご", "メロン", "いちご", "ぶどう"],
    }
  },
  */
  data() {
  return {
      images: [
        { index: 1,
          src: "https://drive.google.com/uc?export=view&id=1IR24pMQ6-A1cgiSEhIIR7p5TwPnqr5no"
        },
        { index: 2,
          src: "https://drive.google.com/uc?export=view&id=1IR24pMQ6-A1cgiSEhIIR7p5TwPnqr5no"
        },
        { index: 3,
          src: "https://drive.google.com/uc?export=view&id=1IR24pMQ6-A1cgiSEhIIR7p5TwPnqr5no"
        },
        { index: 4,
          src: "https://drive.google.com/uc?export=view&id=1IR24pMQ6-A1cgiSEhIIR7p5TwPnqr5no"
        },
        { index: 5,
          src: "https://drive.google.com/uc?export=view&id=1IR24pMQ6-A1cgiSEhIIR7p5TwPnqr5no",
        },
        { index: 6,
          src: "https://drive.google.com/uc?export=view&id=1IR24pMQ6-A1cgiSEhIIR7p5TwPnqr5no"
        },
      ],
      images2: [
        { 
          index:1,
          image: "https://drive.google.com/uc?export=view&id=1IR24pMQ6-A1cgiSEhIIR7p5TwPnqr5no"
        },
      ]
    }
  }

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
  width:550px;
  height:970px;
  margin:auto
}
.beans1 {
    position: absolute;
    top: 170px;
    left: 170px;
}
.beans2 {
    position: absolute;
    top: 300px;
    left: 300px;
}
.beans3 {
    position: absolute;
    top: 350px;
    left: 200px;
}
.beans4 {
    position: absolute;
    top: 400px;
    left: 400px;
}
.beans5 {
    position: absolute;
    top: 150px;
    left: 400px;
}
.beans6 {
    position: absolute;
    top: 400px;
    left: 150px;
}
.beans7 {
    position: absolute;
    top: 500px;
    left: 450px;
}
</style>
