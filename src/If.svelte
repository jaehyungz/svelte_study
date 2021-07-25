<script>
	let name = 'jaehyung'
	let toggle = false;
	if(toggle){

	}else{

	}
	
</script>

<button on:click={() => {toggle = !toggle}}>
	toggle
</button>

{#if toggle}
<h1>
	hello {name}!
</h1>
{:else}
<div>
	No name!
</div>
{/if}