<template>
    <div class="search d-flex align-items-center">
        <input type="text" v-model="query" class="mr-1">
        <button class="btn btn-success" @click="search()">Search</button>
    </div>
</template>

<script>
export default {
  data() {
    return {
      query: " "
    };
  },
  methods: {
    search() {
      this.$store.dispatch("search", this.query);
    }
  }
};
</script>