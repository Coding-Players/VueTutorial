<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <!-- <Home data="Hi I am Sudipta!!!"/>
    <ConditionTute data="Conditional Statement"/>
    <ForLoopTute msg="This is For-Loop Tutorial in vue"/> -->
    <MainHome/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import Home from './components/Home.vue'
// import ConditionTute from './components/ConditionTute.vue'
// import ForLoopTute from './components/ForLoopTute.vue'

import MainHome from './components/Home/MainHome.vue'


export default {
  name: 'App',
  components: {
    // HelloWorld,
    // Home,
    // ConditionTute,
    // ForLoopTute
    MainHome
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
  margin: 0;
  padding: 0;
}
</style>
