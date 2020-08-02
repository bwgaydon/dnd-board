<template>
  <div id="app">
    <AppHeader headerTitle="It's Time For Some Muthafuckin D&D"/>
    <AppSidebar/>
    <div id="map-area">
      <GameBoard/>
    </div>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import AppSidebar from './components/AppSidebar.vue'
import GameBoard from './components/GameBoard.vue'

export default {
  name: 'App',
  components: {
    AppHeader,
    AppSidebar,
    GameBoard
  }
}
</script>

<style lang="scss">
body {
  margin:0;
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

    #map-area {
      display:block;
      width:100%;
      height:100%;
      background-color:aliceblue;
    }
  }
}
</style>
