<script lang="ts">
	let number = 0;

	const randomNumber = () => {
		number = Math.ceil(Math.random() * 100);
	};
</script>

<div class="grid h-full w-full place-items-center">
	<div
		class="grid w-full max-w-sm place-items-center gap-4 rounded-md bg-blue-700 px-8 py-4 shadow-md shadow-zinc-950"
	>
		<h1 class="font-semibold text-zinc-200">Random Number Generator</h1>
		<span class="text-4xl text-zinc-200">{number}</span>
		<hr class="h-0.5 w-full bg-zinc-300" />
		<div class="grid place-items-center gap-4">
			<button type="button" class="rounded bg-zinc-300 px-6 py-4" on:click={randomNumber}>
				Generate
			</button>
		</div>
	</div>
</div>
