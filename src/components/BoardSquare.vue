<template>
  <div class="board-square">
  </div>
</template>

<script>
  export default {
    name: 'BoardSquare'
  }
</script>

<style scoped lang="scss">
.board-square {
	grid-column-start: auto;
  grid-row-start: auto;
  background-size: 100% 100%;
  background-image:
    linear-gradient(to left, grey 1px, transparent 1px),
    linear-gradient(to top, grey 1px, transparent 1px);
  cursor:pointer;
  &:hover,
  &:focus {
    background-color:#cfeeff;
  }
  &:active {
    background-color:#90d9ff;
  }
}
</style>
