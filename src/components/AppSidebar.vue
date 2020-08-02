<template>
  <div class="app-sidebar">
    <button class="sidebar-button">3x3 Board</button>
    <button class="sidebar-button">4x4 Board</button>
  </div>
</template>

<script>
export default {
  name: 'AppSidebar'
}
</script>

<style scoped lang="scss">
.app-sidebar {
  grid-column:1;
  grid-row:2 / 3;
  background-color:#F0F0F0;
  padding:32px 16px;

  .header-logo-img {
    height:100%;
    width:auto;
    margin-right:32px;
  }
  .sidebar-button {
    height:40px;
    width:auto;
    margin:0 24px 24px 24px;
    color:#ffffff;
    background-color:#087762;
    border:none;
    border-radius:5px;
  }
}
</style>
