<script setup>
import Load from "./components/Load.vue";
import Background from "./components/Background.vue";
import Daily from "./components/Daily.vue";
import Signature from "./components/Signature.vue";
</script>

<template>
	<header class="header">
		<Load />
		<Background />
		<Signature />
	</header>
	<Daily />
</template>

<style scoped>
.header {
	position: relative;
	height: 100dvh;
	width: 100%;
}
</style>
