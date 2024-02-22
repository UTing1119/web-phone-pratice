<template>
  <div class="foot-container">
    <template v-for="t in text">
      <Tag :text="t" />
    </template>
    <span class="text">點讚</span>
    <span class="text">收藏</span>
    <span class="text">評論</span>
    <span class="text">觀看</span>
  </div>
</template>

<script setup lang="ts">
import Tag from './Tag.vue';
import { PropType } from 'vue';

defineProps({
  text: {
    type: Array as PropType<String[]>,
    default: []
  }
})

</script>

<style scoped>
.foot-container{
  display: flex;
  flex-direction: row;
  gap: 4px;
}
.text{
  color: #666;
  font-size: 0.8em;
}
</style>