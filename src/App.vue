<template>
  <div id="app">
    <search></search>
    <results></results>
  </div>
</template>

<script>
import Search from './Search.vue'
import Results from './Results.vue'

export default {
  name: 'app',
  components: {Search, Results}
}
</script>
