<template>
	<div class="card" style="width: 22rem;">
		<div class="card-body">
			<span class="card-title">標題</span>
			<div class="main-content">
				<Content class='content' />
				<div class="pic"></div>
			</div>
			<Footer :text="text" />
		</div>
	</div>
</template>

<script setup lang="ts">
import Content from './Content.vue';
import Footer from './Footer.vue';
import { type PropType } from 'vue';

defineProps({
  text: {
    type: Array as PropType<string[]>,
    default: []
  },
})
</script>

<style scoped>
.card-title{
	font-size: 24px;
	font-weight: bold;
}

.main-content{
	display: flex;
	justify-content: center;
	align-items: center;
	flex-wrap: wrap;
	gap: 16px;
}

.content{
	width: 60%;
}
.content-max{
	width: 100%;
}

.pic{
	background-color: #666;
	height: 100px;
	width: 100px;
	border-radius: 8px;
}

</style>