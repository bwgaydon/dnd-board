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
  border:1px solid #2c3e50;
}
</style>
