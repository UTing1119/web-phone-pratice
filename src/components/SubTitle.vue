<template>
	<div class="container">
		<div class="avator"></div>
		<span class="p-2 name">name</span>
		<span class="p-2 date">2024-02-22</span>
	</div>
</template>

<script setup lang="ts">

</script>

<style scoped>
.avator{
	background-color: #666;
	border:  5px solid #666;
	width: 20px;
	height: 20px;
	border-radius: 100px;
}

.container{
	display: flex;
	flex-direction: row;
	justify-content: start;
	align-items: center;
	gap: 8px;
}

.name{
	font-size: 1.1em;
}
.date{
	color: #666;
	font-size: 0.9em;
}
</style>