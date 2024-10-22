<script setup>
import { ref, onMounted } from "vue";

const positionStyle = ref("fixed");

onMounted(() => {
	setTimeout(() => {
		positionStyle.value = "absolute";
	}, 3000);
});
</script>
<template>
	<h1 class="signature" :style="{ position: positionStyle }">
		<span> A </span>
		<span> r </span>
		<span> t </span>
		<span> e </span>
		<span> m </span>
		<span> i </span>
		<span> s </span>
		<span> a </span>
	</h1>
</template>
<style scoped>
.signature {
	position: fixed;
	top: 50%;
	left: 50%;
	width: 100%;
	z-index: 3;
	transform: translateX(-50%) translateY(-50%);
	color: #fff;
	font-family: "Rusillaserif";
	text-align: center;
	font-size: 4.2rem;
	font-weight: 100;
	text-shadow: 4px 2px 3px #000;
	animation: textAnimation 3s cubic-bezier(0.695, 0.245, 0, 0.98) forwards 0.5s, all 0.3s;
}

.signature span {
	display: inline-block;
	transform: scale(0) rotate(90deg);
	filter: drop-shadow(0px 0px 25px #fff);
	animation: scaleUp 0.5s forwards cubic-bezier(0.1, 0.245, 0.1, 0.1);
}

.signature span:nth-child(1) {
	animation-delay: 0.1s;
}
.signature span:nth-child(2) {
	animation-delay: 0.2s;
}
.signature span:nth-child(3) {
	animation-delay: 0.3s;
}
.signature span:nth-child(4) {
	animation-delay: 0.4s;
}
.signature span:nth-child(5) {
	animation-delay: 0.5s;
}
.signature span:nth-child(6) {
	animation-delay: 0.6s;
}
.signature span:nth-child(7) {
	animation-delay: 0.7s;
}
.signature span:nth-child(8) {
	animation-delay: 0.8s;
}

@keyframes scaleUp {
	0% {
		transform: scale(0) rotate(60deg);
	}

	80% {
		transform: scale(0.8) rotate(-20deg);
	}

	100% {
		transform: scale(1) rotate(0deg);
	}
}

@keyframes textAnimation {
	0% {
	}

	100% {
		font-size: 3rem;
		top: 2rem;
	}
}
</style>
