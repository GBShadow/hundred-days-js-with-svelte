<script lang="ts">
	let color = '#ffffff'

	const randomHexColor = () => {
		color = '#' + Math.random().toString(16).substring(2,8)
	}
</script>


<div class="grid h-full w-full place-items-center">
	<div
		class="grid w-full max-w-sm place-items-center gap-4 rounded-md bg-blue-700 py-4 px-8 shadow-md shadow-zinc-950"
	>
		<h1 class="font-semibold text-zinc-200">Random Hex Color Generator</h1>
		<div class="flex gap-4 items-center">
			<span class="text-4xl text-zinc-200">{color}</span>
			<div class="h-8 w-8" style="background-color: {color}"/>
		</div>
		<hr class="h-0.5 w-full bg-zinc-300" />
		<div class="grid place-items-center gap-4">
			<button type="button" class="px-6 py-4 bg-zinc-300 rounded" on:click={randomHexColor}> Generate Color </button>
		</div>
	</div>
</div>
