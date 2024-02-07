<script>
	import '../app.pcss';
	import Sidebar from '$lib/components/sidebar.svelte'
</script>

<div class="h-screen w-screen bg-zinc-900 overflow-hidden flex">
	<Sidebar />
	<slot />
</div>
