<script>
let name = $state('Атэц');
let count = $state(0);
</script>

<div class="min-h-screen bg-zinc-950 text-zinc-50 flex items-center justify-center p-8">
	<div class="w-full max-w-96 flex flex-col gap-8 justify-center items-center text-pink-500">
		<h1 class="font-semibold tracking-tight text-7xl text-yellow-500 text-center">Hello {name}🤘</h1>
		
		<input
			bind:value={name}
			class="flex h-10 w-full rounded-md border border-zinc-800 bg-zinc-900 px-3 py-2 placeholder:text-zinc-400 focus:outline-none focus:ring-2 focus:ring-zinc-700 focus:ring-offset-2 focus:ring-offset-zinc-950 text-yellow-500"
			placeholder="Enter your name"
		/>
		
		<button
			onclick={() => count += 1}
			class="inline-flex h-10 items-center justify-center rounded-md px-4 py-2 text-sm font-medium text-zinc-900 transition-colors hover:bg-zinc-200 focus:outline-none focus:ring-2 focus:ring-zinc-700 focus:ring-offset-2 focus:ring-offset-zinc-950 bg-yellow-500"
		>
			Clicks: {count}
		</button>
	</div>
</div>
