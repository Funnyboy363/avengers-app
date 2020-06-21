<template>
<div>
  <div id="app">
    <h1>Avengers <br>Playground<br> App</h1>
    <p class="clickbuttons">Click on the Names to Switch images</p>
    <HelloWorld />
    <p class="bottom"></p>
    <Avengers />
  <p class="bottom"></p>
  </div>
  <div class="text-center bottom">
  <iframe src="https://www.youtube.com/embed/TcMBFSGVi1c" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </div>
  <p class="bottom"></p>
</div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import Avengers from './components/Avenger.vue';
export default {
  name: 'App',
  components: {
    HelloWorld,
    Avengers
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

h1 {
  width: 100%;
  background-image: url('https://i.pinimg.com/originals/4f/75/2c/4f752cc6a81e5f3cb904536d03f53b4b.jpg');
  background-size: cover;
  padding: 120px 0;
  color: rgb(197, 197, 197);
  font-weight: 700;
  font-size: 70px;
  text-align: left;
  padding-left: 160px;
  margin-bottom: 0;
}

p.clickbuttons {
background-color: rgb(30, 0, 70);
padding: 10px 0;
margin: 0;
color: white;
}

   
.bottom {
padding: 20px 0;
}


iframe {
  width: 70%;
  height: 500px;
}

</style>
