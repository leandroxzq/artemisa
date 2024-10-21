<script setup>
import { ref, onMounted } from "vue";

const isVisible = ref(true);

onMounted(() => {
	setTimeout(() => {
		isVisible.value = false;
	}, 4000);
});
</script>

<template>
	<div class="load" v-if="isVisible"></div>
</template>

<style scoped>
.load {
	position: fixed;
	height: 100vh;
	width: 100vw;
	z-index: 2;
	max-width: 1280px;
	background: #000000;
	animation: upNone 3s cubic-bezier(0.695, 0.245, 0, 0.98) forwards 1s;
}

@keyframes upNone {
	0% {
	}
	100% {
		background: #00000000;
	}
}
</style>
