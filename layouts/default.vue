<template>
	<div class="main-container">
		<Topbar/>
		<div class="app">

			<Nuxt />

		</div>
	</div>
</template>

<script>
	import Topbar from '@/components/topbar'

	export default {
		
		components: {
			Topbar,
		}
	}
</script>

<style scoped>
	html {
		font-family:
			'Montserrat',
			Arial,
			sans-serif;
		margin: 0;
	}

	*,
	*::before,
	*::after {
		margin: 0;
		padding: 0;
	}

	.main-container {
		background: #FCFCFC;
	}

	.app {
		height: 100vh;
		width: 100vw;
	}
</style>
