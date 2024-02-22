<template>
  <div class="list-container">
    <div class="container-fluid">
    <span class="navbar-brand mb-0 h1">文章</span>
    </div>
    <Card 
      :text="['美文', '故事', '精選優質']"
    />
    <Card
      :text="['日文', '文章']"
      :pic="3"
    />
  </div>
</template>

<script setup lang="ts">
import Card from '@/components/Card.vue';
</script>

<style scoped>
.container-fluid{
  text-align: center;
  background-color: #333;
  color: white;
  font-weight: bold;
}

.list-container{
  display: flex;
  flex-direction: column;
  gap: 16px;
}
</style>