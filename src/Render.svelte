<script>
	let name = 'kid'
	let age = 26

function assign() {
		 name = 'jaehyungz';
		 age = 27;
}
	
</script>

<main>
	<h1>Hello {name}!</h1>
	<h2 class={age > 25 ? "active" : ''}>
		{age}
	</h2>
	<img src='' alt={name}/>
	<input type='text' bind:value={name}/>
	<button on:click={assign}>assign</button>
	
</main>

<style>
	h1{
		color:red
	}
	.active{
	color:blue
	}
</style>