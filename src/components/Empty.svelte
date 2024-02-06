<script lang="ts">
	let show: boolean = false;
	const showChild = () => {
		show = true;
	}
</script>

<div class="wrap">
	{#if show === true}
		<p>子要素</p>
	{/if}
</div>
<button on:click={showChild}>子要素表示</button>

<style>
	.wrap {
		padding: 20px;
		&:empty {
			width: 20px;
			height: 20px;
			background-color: pink;
		}
	}
</style>