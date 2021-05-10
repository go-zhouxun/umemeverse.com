<template>
  <div id="app">
    <div class="nav">
      <router-view/>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 30px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.nav {
  height: 25px;
  width: 100%;
}

body {
  padding: 0;
  margin: 0;
  height: 100%;
  min-height: 100vh;
  min-width: 360px;
  background-color: #2A3253;
}
</style>
