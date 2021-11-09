<script>
	let count = 0;
	$: double = count * 2;

	function countClick () {
		count++
		
	}

	$: {
		console.log(double + count)
		
	}
</script>

<button on:click={countClick}>Ты нажал {count} раз а это повтор кода {double}</button>


