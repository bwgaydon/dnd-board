<template>
  <div id="app">
    <AppHeader/>
    <AppSidebar/>
    <GameBoard/>
  </div>
</template>

<script lang="js" src="./app.js"></script>

<style lang="scss">
body {
  margin:0;
  * {
    box-sizing:border-box;
  }

  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    display:grid;
    width:100vw;
    height:100vh;
    grid-template-columns: 360px auto;
    grid-template-rows: 100px auto;
  }
  
}
</style>
