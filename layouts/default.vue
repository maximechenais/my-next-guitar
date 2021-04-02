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

<style>
    html {
        font-family: 'Montserrat';
        margin: 0;
        width: 100%;
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