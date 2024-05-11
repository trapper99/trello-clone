<template>
  <main>
    <h1>Build a Trello Clone Home Page</h1>
    <pre>{{ boardStore.board }}</pre>
  </main>
</template>

<script lang="ts">
import Vue from 'vue'
import { useBoardStore } from '~/store/boardStore';

export default Vue.extend({
  name: 'IndexPage',
  setup() {
    const boardStore = useBoardStore();

    return {
      boardStore,
    }
  }
})
</script>
