<template>
  <div>{{ fullName }}</div>
</template>

<script lang="ts">
export default {
  name: 'E02Reactive'
}
</script>

<script setup lang="ts">
import { reactive, computed, onMounted } from 'vue'

const state = reactive({
  firstName: 'Kyungsu',
  lastName: 'Lee'
})

const fullName = computed(() => state.firstName + ' ' + state.lastName)

onMounted(() => {
  setTimeout(() => {
    state.firstName = 'KSL'
  }, 2000)
})
</script>

<style scoped>
</style>
