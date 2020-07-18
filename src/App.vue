<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <!-- <DataBind /> -->
    <Child v-bind:users="users" />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import DataBind from "./components/DataBind";
import Child from "./components/Child";
export default {
  name: "App",
  components: {
    // HelloWorld
    // DataBind
    Child
  },
  data() {
    return {
      users: [
        { name: "Hello", email: "hello@test.com" },
        { name: "World", email: "world@test.com" },
        { name: "Vue", email: "vue@test.com" },
        { name: "React", email: "react@test.com" }
      ]
    };
  }
};
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
