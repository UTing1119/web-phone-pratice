<template>
  <span class="badge text-bg-primary">
    {{ text }}
  </span>
</template>

<script setup lang="ts">
defineProps({
  text: {
    type: String,
    default: ''
  }
})
</script>

<style scoped>
.badge{
  border: 1px solid #333;
  border-radius: 4px;
  font-size: 0.7em;
  padding: 2px 4px;
}
</style>