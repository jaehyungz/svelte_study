<script>
	import {onMount} from 'svelte'
	let name ='world'
	let isRed = false;
	
	//현재 화면이 준비가 되면 useEffect와 비슷한 hooks
    // 	onMount(()=>{
    // 		const box = document.querySelector('.box')
    // 		box.addEventListener('click',()=>{
    // 		isRed = !isRed
    // 		})
    // 	})
	
	function handleToggle (){
		isRed = !isRed
	}
	

	
</script>

<h1>
	hello {name}
</h1>
<div class='box' style="background-color: {isRed ? 'red' : 'orange'};"on:click={handleToggle}
		 on:mouseenter={() => name='enter'}
			on:mouseleave={() => name='leave'}>
	BOX
</div>


<style>
	.box{
		width:300px;
		height:150px;
		background-color:orange;
	}
</style>