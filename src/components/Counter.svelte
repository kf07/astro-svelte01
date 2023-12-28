<script lang="ts">
	let count = 0;
	const addCount = () => {
		count++;
	}
</script>

<p>{count}</p>
<button on:click={addCount}>add</button>