<template>
	<main>
		<h1 class="name">Hello {name}!</h1>
		<p>
			maan
			<span>
				some weird stuff
			</span>
		</p>
	</main>
</template>

<script>
	export let name;
</script>

<style lang="less">
	@mycolor: #ff3e00;

	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	.name {
		color: @mycolor;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	p {
		color: red;

		span {
			color: blue;
		}
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
