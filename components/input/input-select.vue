<template>
	<div>
		<label >{{ label }}</label>

		<select>

			<option value="" 
				v-for="{option, index} in options" 
				:key="index"
			>
				{{ option.text }}
			</option>

		</select>
	</div>
</template>

<script>
	export default {
		name: 'inputSelect',

		props: {
			
			label: String,

			options: {
				text: String,
			}
		}

	}
</script>

<style scoped>

</style>