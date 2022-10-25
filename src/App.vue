<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <!-- <calculator/> -->
  <!-- <sri/> -->
  <LoginForm/>
</template>

<script>
// import Login from './components/Login.vue'
// import HelloWorld from './components/HelloWorld.vue'
// import Sri from './components/Sri.vue'
// import calculator from './components/calculator.vue'
// import Add from './components/Add.vue'
import LoginForm from './components/LoginForm.vue'

export default {
  name: 'App',
  components: {
    // Sri,
    LoginForm,
    // calculator
    // Add
    // HelloWorld
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
