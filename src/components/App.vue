<template lang="html">
	<div>
		<button @click="amount++"> Click me </button>
		<br />
		The button has been clicked {{amount}} times.

		<p>
			{{passion}}
		</p>
	</div>
</template>

<script>
console.log('process', process);
console.log('process.env', process.env);
console.log('process.env.SECRET_PASSION', process.env.SECRET_PASSION);

export default {
	data: () => ({
		amount: 0,
		passion: process.env.SECRET_PASSION
	})
}
</script>

<style lang="css" scoped>
button {
	padding: 1em;
	border-radius: 1em;
}
</style>
