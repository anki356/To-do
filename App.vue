<template>
  <div id="app">
    
  <todo></todo>
  </div>
</template>

<script>
/*import HelloWorld from './components/HelloWorld'*/
import todo from './components/todo'

export default {
  name: 'App',
  components: {
    todo
  }
}
</script>

<style>
*{
  box-sizing: border-box;}

  .container{
    max-width: 600px;
    margin : @ auto;
  }
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /*text-align: center;*/
  color: #2c3e50;
  margin-top: 60px;
}
</style>
