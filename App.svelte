<script>
let name = $state('Curva');
let count = $state(0);
</script>

<div class="min-h-screen bg-zinc-950 text-zinc-50 flex items-center justify-center p-8">
	<div class="w-full max-w-sm space-y-6">
		<h1 class="text-2xl font-semibold tracking-tight">Hello {name}!</h1>
		
		<input
			bind:value={name}
			class="flex h-10 w-full rounded-md border border-zinc-800 bg-zinc-900 px-3 py-2 text-sm placeholder:text-zinc-400 focus:outline-none focus:ring-2 focus:ring-zinc-700 focus:ring-offset-2 focus:ring-offset-zinc-950"
			placeholder="Enter your name"
		/>
		
		<button
			onclick={() => count += 1}
			class="inline-flex h-10 items-center justify-center rounded-md bg-zinc-50 px-4 py-2 text-sm font-medium text-zinc-900 transition-colors hover:bg-zinc-200 focus:outline-none focus:ring-2 focus:ring-zinc-700 focus:ring-offset-2 focus:ring-offset-zinc-950"
		>
			Clicks: {count}
		</button>
	</div>
</div>
