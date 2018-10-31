<template>
    <div class="results">
        <div class="item" v-for="(item, index) in results" v-bind:key="index">
            <a :href="item.url" class="item-title">{{item.title}}</a>
            <div class="item-url">
                {{ item.url }}
            </div>
            <div class="item-snippets" v-html="item.snippet"></div>
        </div>
    </div>
</template>

<script>
export default {
  computed: {
    results() {
      return this.$store.getters.results;
    }
  }
};
</script>