<template>
  <div id="app">
    <HelloWorld />
    <br />
    <ButtonHoge />
    <br />
    <SpTodo />
<!-- <router-view/> -->
  </div>
</template>

<script>
import HelloWorld from './components/sample_hoge/HelloWorld'
import ButtonHoge from './components/sample_button/ButtonHoge'
import SpTodo from './components/sample_todo/SpTodo'
export default {
  name: 'App',
  components: {SpTodo, ButtonHoge, HelloWorld}
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
