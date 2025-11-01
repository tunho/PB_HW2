<template>
  <div>Hello, {{ message }}</div>
</template>

<script lang="ts">
export default {
  name: 'E01Instance'
}
</script>

<script setup lang="ts">
import { reactive } from 'vue'

const state = reactive({
  message: 'Vue!'
})

const message = state.message
</script>

<style scoped>
div {
  color: blue;
}
</style>
