<template>
<div class="kanban-container">
  <div class="kanban-board" v-for="board in boards" :key="board.name">
    {{board.name}}
  </div>
</div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  },
  data: function() {
    return {
      boards: [{ name: "board1" }, { name: "board2" }, { name: "board3" }]
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.kanban-container {
  display: flex;
  margin: 0 auto;
  justify-content: space-around;
}
.kanban-board {
  min-height: 300px;
  width: 300px;
  background-color: #cccccc;
}
</style>
