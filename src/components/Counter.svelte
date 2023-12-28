<script lang="ts">
	let count: number = 0;
	const addCount = () => {
		count++;
	}
	$: count1 = count + 5;
</script>

<p>{count}</p>
<button on:click={addCount}>add</button>
<p>{count1}</p>
<p>deploy test</p>