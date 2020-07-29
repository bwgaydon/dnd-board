<template>
  <div class="game-board">
    <BoardSquare v-for="square in this.boardSquares" :key="square.id"/>
  </div>
</template>

<script>
  import BoardSquare from '../components/BoardSquare.vue'

  export default {
    name: 'GameBoard',
    data () {
      return {
        boardDimensions: {
          x: 4,
          y: 4
        },
        boardSquares: [
          {
            id: 1,
            bgColor: 'blue'
          },
          {
            id: 2,
            bgColor: 'red'
          },
          {
            id: 3,
            bgColor: 'blue'
          },
          {
            id: 4,
            bgColor: 'red'
          },
          {
            id: 5,
            bgColor: 'blue'
          },
          {
            id: 6,
            bgColor: 'red'
          },
          {
            id: 7,
            bgColor: 'blue'
          },
          {
            id: 8,
            bgColor: 'red'
          }
        ]
      }
    },
    components: {
      BoardSquare
    }
  }
</script>

<style scoped lang="scss">
.game-board {
	//position:fixed;
	//width:100vw;
	//height:100vh;
	background:aliceblue;
  z-index:0;
  display:grid;

  --rowCount: 4;
  --colCount: 4;
  grid-template-rows: repeat(var(--rowCount), 40px);
  grid-template-columns: repeat(var(--colCount), 40px);
}
</style>
