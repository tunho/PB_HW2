<template>
  <div>
    <p>Name: {{ person.name }}</p>
    <p>Age: {{ person.age }}</p>
    <button @click="incrementAge">Increment Age</button>
  </div>
</template>

<script lang="ts">
export default {
  name: 'E11Reactive'
}
</script>

<script setup lang="ts">
import { reactive } from 'vue'

const person = reactive({
  name: 'John Doe',
  age: 30
})

const incrementAge = () => {
  person.age++
}
</script>

<style scoped>
</style>
