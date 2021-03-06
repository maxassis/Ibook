<template>
  <div class="book-list">
    <h2>Listagem de Livros</h2>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({});
</script>

<style lang="scss" scoped>
.book-list {
  display: grid;
  grid-template-columns: repeat(6, 1fr);
  grid-template-rows: auto;
  grid-gap: 2rem;
  @include screen("small") {
    grid-template-columns: repeat(2, 1fr);
  }
  @include screen("medium") {
    grid-template-columns: repeat(3, 1fr);
  }
}
</style>
