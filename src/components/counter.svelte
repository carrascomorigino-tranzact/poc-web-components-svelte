<svelte:options tag={null} />

<script>
	let count = 0;

	function inc() {
		count++;
	}

	function dec() {
		count--;
	}
</script>

<style>
	* {
		font-size: 200%;
	}

	span {
		width: 4rem;
		display: inline-block;
		text-align: center;
	}

	button {
		width: 64px;
		height: 64px;
		border: none;
		border-radius: 10px;
		background-color: seagreen;
		color: white;
	}
</style>

<button on:click={dec}>
	-
</button>
<span>{count}</span>
<button on:click={inc}>
	+
</button>