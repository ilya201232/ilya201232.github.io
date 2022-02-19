<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <div>
    <div v-for="data in myJson" v-bind:key="data">{{data}}</div>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import json from './json/data.json'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data(){
    return {
      myJson: json
    }
  }
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
</style>
