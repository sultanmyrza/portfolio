<template>
  <div>
    <h2>
      {{ header }}
    </h2>
    <ul>
      <li v-for="item in items" :key="item">
        {{ item }}
      </li>
    </ul>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  props: {
    header: {
      type: String,
      default: () => 'Header'
    },
    items: {
      type: Array,
      default: () => []
    }
  }
})
</script>

<style scoped>
ul {
  list-style: none;
}
ul > li::before {
  content: '✅';
}
</style>
