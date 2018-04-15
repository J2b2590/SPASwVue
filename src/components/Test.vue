<template>
	<div class='test'>
		<input type='text' v-model="title"><br />
		<h1>{{title}}</h1>
		<p v-if='showName'>{{user.firstName}}</p>
		<p v-else>nobody</p>
		<ul>
			<li v-for='item in items'>{{item.title}}</li>
		</ul>
		<button v-on:click="greeting('Hello World')"> say greeting</button>
		<br />
		<input type='text' v-on:keyup="pressKey">
	</div>
</template>


<script>
	export default {
		name: 'test',
		data() {
			return {
				title: "Hello World",
				user: {
					firstName: 'Jon',
					lastName: 'Doe'
				},
				showName: true,
				items: [
				{title:'Item One'},
				{title:'Item Two'},
				{title:'Item Three'},
				]
			}
		},
		methods: {
			greeting: function(greet){
				alert(greet)
			},
			pressKey: function(e){
				console.log(e.target.value);
			}
		}
	}
</script>


<style scoped>

</style>