<template>
	<div class='users'>
	<h1>Users</h1>
		
	</div>
</template>


<script>
	export default {
		name: 'users',
		
		data() {

			return {
				users: [
				{
					name: "Jon Doe",
					email: "jdoe@gmail.com",
					contacted: false
				},
				{
					name: "Jane Doe",
					email: "JaneDoe@gmail.com",
					contacted: false
				},
				{
					name: "Hale Johnston",
					email: "HaleJohn@gmail.com",
					contacted: false
				}
			]
				
		}
	},
		methods: {
			
		},
		
	}
</script>


<style scoped>

</style> 