<script setup></script>
<template>
	<header class="header">
		<div class="header__background"></div>
		<!--<h1 class="header__signature">Artemisa</h1> -->
	</header>
</template>
<style>
.header {
	position: relative;
	height: 100dvh;
	width: 100%;
}

.header__background {
	position: absolute;
	height: 100dvh;
	width: 100%;
	background: url(../assets/img/5EC79C09-078A-4BB3-B482-651709977CAC.jpg);
	background-repeat: no-repeat;
	background-position: center 20%;
	background-size: cover;
}

.header__signature {
	position: absolute;
	width: 100%;
	top: 1rem;
	font-family: "Rusillaserif";
	text-align: center;
	font-size: 3rem;
	color: #fff;
	font-weight: 100;
	text-shadow: 2px 3px 1px #000;
}
</style>
