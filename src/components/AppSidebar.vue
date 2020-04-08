<template>
  <div class="app-sidebar">
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
  padding:16px;

  .header-logo-img {
    height:100%;
    width:auto;
    margin-right:32px;
  }
  .header-title {
  }
}
</style>
