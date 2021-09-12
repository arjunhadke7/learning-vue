<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Hello world" />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  // the name is app, and the component being called here is HelloWorld
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
