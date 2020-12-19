<template>
	<header class="header">
		<p class="header-color">{{color}}</p>
	</header>
</template>

<script>
export default {
	name: 'Header',
	props: {
		color: String
	}
}
</script>

<style scoped>
	.header {
		width: 100%;
		background-color: #fff;
		text-align: center;
		padding: 1rem 0;
    font-weight: bold;
    font-size: 1.1rem;
	}
</style>