<template>
  <div class="game-board">
    <BoardSquare v-for="square in this.boardSquares" :key="square.id"/>
  </div>
</template>

<script>
  import BoardSquare from '../components/BoardSquare.vue'

  export default {
    name: 'GameBoard',
    methods: {
      handleScroll: function (event) {
        console.log(event)
      }
    },
    data () {
      return {
        boardDimensions: {
          x: 3,
          y: 3
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
          },
          {
            id: 9,
            bgColor: 'blue'
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
  z-index:0;
  display:grid;
  background-color:#faf9f0;

  --rowCount: 3;
  --colCount: 3;
  grid-template-rows: repeat(var(--rowCount), 40px);
  grid-template-columns: repeat(var(--colCount), 40px);
}
</style>
