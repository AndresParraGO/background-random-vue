<template>
	<button class="btn" v-on:click="$emit('cambiar-fondo', changeColor())">
		<img class="btn-icon" alt="Icon Arrow Right" src="https://www.participe-amstelland.nu/public/images/user/arrow.right.svg" />
	</button>
</template>

<script>
export default {
	name: 'BtnChangeBackground',
	methods: {
    changeColor: function() {
      return '#' + Math.floor(Math.random() * 6777215).toString(16);
    }
  }
}
</script>

<style scoped>
	.btn {
		position: absolute;
		top: 50%;
		right: 0;
		transform: translateY(-50%);

		padding: 3rem 1rem;
		border: none;
		color: #fff;
		cursor: pointer;
		transition: all 300ms linear;
	}
	.btn:hover {
		background-color: #222;
	}
	.btn:focus {
		outline: none;
	}
	.btn-icon {
		width: 30px;
	}
</style>