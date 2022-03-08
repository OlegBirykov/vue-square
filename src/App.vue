<template>
  <div class="columns is-multiline cells-container">
    <div class="column is-2 cell" v-for="n in 36" :key="n">
      <Cell state />
    </div>
  </div>
</template>

<script>
import Cell from "./components/Cell.vue";

export default {
  name: "App",
  components: {
    Cell,
  },
};
</script>

<style lang="scss">
@import "bulma/bulma.sass";

$size: 70px;

.body {
  background-color: lightgray;
}

#app {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;

  display: flex;
  justify-content: center;
  align-items: center;
}

.columns.cells-container {
  width: $size * 6;
  margin: auto;
}

.column.cell {
  padding: 0;
}
</style>
