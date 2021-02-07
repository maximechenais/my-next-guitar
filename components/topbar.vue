<template>
	<div class="main-container">

		<img src="@/assets/icons/main-logo.svg" alt="website-logo">

		<h1>“one guitar is good, more than one is better”</h1>

	</div>
</template>

<script>
	export default {
		name: 'Topbar',
	}
	
</script>

<style scoped>
	.main-container {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		align-items: center;
		height: 77px;
		padding: 0 150px 0 40px;
		font-family: 'Righteous';
	}

	.main-container img {
		width: 383px;
		height: 75px;

	}

	.main-container h1 {
		font-size: 24px;
		font-weight: 500;
		color: #56C5CC;
	}

</style>