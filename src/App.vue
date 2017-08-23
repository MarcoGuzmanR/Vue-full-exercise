<template>
  <div id="app">
    <img src="./assets/logo.png">
    <!-- <login></login> -->
    <register></register>
    <!-- <stories :stories='stories'></stories> -->
  </div>
</template>

<script>
// import Login from './components/Login';
import Register from './components/Register';
// import Stories from './components/Stories';

export default {
  name: 'app',
  components: {
    // Login,
    Register,
    // Stories,
  },
};
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
