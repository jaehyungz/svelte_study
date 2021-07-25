<script>
	let name ='FRUITS'
	let furits =['🍎','🍌','🍒',"🍊",'🥭']
	function deleteFruit(){
	furits =furits.slice(1)
}
</script>

<h1>
	hello {name}
</h1>
<ul>
{#each furits as fruit}
	<li>{fruit}</li>
{/each}	
</ul>
<button on:click={deleteFruit}>
	Eat it!
</button>