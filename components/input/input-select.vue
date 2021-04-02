<template>
	<div>
		<label >{{ label }}</label>

		<select>

			<option 
			>
			</option>

		</select>
	</div>
</template>

<script>
    export default {
        name: 'inputSelect',

        props: {

            label: String,

            brandList: Object,
        }

    }
</script>

<style scoped>

</style>