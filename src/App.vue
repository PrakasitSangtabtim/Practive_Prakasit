<template>
  <div id="app">
    <router-link to="/">Home</router-link> |
    <router-link to="/vmodel">V-model</router-link> |
    <router-link to="/von">V-no</router-link> |
    <router-link to="/vbind">V-bind</router-link> |
    <router-link to="/vif">V-if</router-link> |
    <router-link to="/vfor">V-for</router-link> |
    <router-link to="/prop">Prop</router-link> |
    <router-link to="/axios">Axios</router-link>
    <br />

    <router-view />
  </div>
</template>

<script>
export default {
  name: "App",
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>


