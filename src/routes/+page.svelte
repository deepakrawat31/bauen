<script lang="ts">
	import { ArrowUpRight, MoveUpRight } from 'lucide-svelte';
</script>

<svelte:head>
	<title>Bauen</title>
</svelte:head>

<main class="flex flex-col gap-0.5 lg:flex-row">
	<section class="flex min-h-dvh flex-1 flex-col gap-8">
		<header class="flex p-4">
			<span class="text-9xl lowercase">bauen</span>
		</header>
		<div class="flex flex-1 flex-col gap-8 p-4">
			<p class="font-pitagon text-sm leading-loose font-bold md:text-base">
				<em class="text-emerald-400">bauen</em>, German for
				<em class="text-emerald-400">"to build"</em>, curates custom playlist based on your most
				played spotify tracks.
			</p>
			<button class="font-pitagon group flex w-fit gap-1 leading-none font-bold uppercase">
				<span class="rounded bg-neutral-800 p-4">link spotify</span>
				<span class="relative isolate overflow-hidden rounded bg-neutral-800 p-3">
					<span
						class="absolute -top-1/2 -left-1/2 -z-20 aspect-square h-40 scale-0 rounded-full bg-emerald-400 transition-transform duration-500 group-hover:scale-100"
					></span>
					<MoveUpRight
						size={24}
						class="transition-colors duration-500 group-hover:text-neutral-900"
					/>
				</span>
			</button>
		</div>
		<nav class="flex items-end gap-6 p-4">
			<a href="/"><img src="/favicon.webp" alt="favicon" class="size-6" /></a>
			<a
				href="/"
				class="font-pitagon flex items-end gap-1 leading-tight uppercase transition-colors duration-300 hover:text-emerald-400"
			>
				<span>github</span>
				<ArrowUpRight />
			</a>
			<a
				href="/"
				class="font-pitagon flex items-end gap-1 leading-tight uppercase transition-colors duration-300 hover:text-emerald-400"
			>
				<span>mail</span>
				<ArrowUpRight />
			</a>
		</nav>
	</section>
	<section
		class="grid min-h-dvh w-full grid-cols-2 grid-rows-2 bg-emerald-800 lg:max-w-xl"
	></section>
</main>
