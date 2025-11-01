<template>
  <div>
    <ChildComponent1 />
  </div>
</template>

<script lang="ts">
export default {
  name: 'E06ParentComponent'
}
</script>

<script setup lang="ts">
import { provide } from 'vue'
import ChildComponent1 from '@/components/example4/ChildComponent1.vue'

provide('sharedMessage', 'Hello from provide')
</script>

<style scoped>
</style>
