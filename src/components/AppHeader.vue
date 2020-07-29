<template>
  <header class="app-header">
    <img class="header-logo-img" src="../assets/logo.png" />
    <h1 class="header-title">It's Time For Some Muthafuckin' D&D</h1>
  </header>
</template>

<script lang="js" src="./app_header.js"></script>

<style scoped lang="scss">
.app-header {
  grid-column:1 / 3;
  grid-row:1;
  display:flex;
  flex-direction:row;
  flex-wrap:nowrap;
  justify-content: flex-start;
  align-items:center;
  background-color:#087762;
  padding:16px;
  z-index:2;

  .header-logo-img {
    height:100%;
    width:auto;
    margin-right:32px;
  }
  .header-title {
    display:inline-block;
  }
}
</style>
