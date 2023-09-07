<script>
	export let side
	export let quarter = ''
	export let points = []
</script>

{#if side === 'left'}
	<div class="w-full px-4 md:w-1/2">
		<div class="relative z-10 mb-10 rounded-lg py-8 px-6 bg-dark md:mr-3 md:mb-0 md:text-right lg:mr-5">
			<span class="absolute top-1/2 left-0 hidden h-4 w-4 -translate-y-1/2 rounded-full border-4 border-body-color bg-primary md:left-auto md:-right-9 md:block lg:-right-11"></span>
			<span class="absolute -right-1 top-1/2 hidden h-3 w-3 -translate-y-1/2 rotate-45 bg-dark md:block"></span>

			<h3 class="mb-3 text-xl font-bold text-white">{quarter}</h3>

			{#each points as point}
				<p class="mb-5 text-base font-medium text-body-color">{point}</p>
			{/each}
		</div>
	</div>
	<div class="w-full px-4 md:w-1/2"></div>
{:else if side === 'right'}
	<div class="w-full px-4 md:w-1/2"></div>
	<div class="w-full px-4 md:w-1/2">
		<div class="relative z-10 mb-10 rounded-lg py-8 px-6 bg-dark md:ml-3 md:mb-0 lg:ml-5">
			<span class="absolute top-1/2 left-0 hidden h-4 w-4 -translate-y-1/2 rounded-full border-4 border-body-color bg-primary border-body-color md:right-auto md:-left-9 md:block lg:-left-11"></span>
        	<span class="absolute -left-1 top-1/2 hidden h-3 w-3 -translate-y-1/2 rotate-45 bg-dark md:block"></span>

			<h3 class="mb-3 text-xl font-bold text-white">{quarter}</h3>

			{#each points as point}
				<p class="mb-5 text-base font-medium text-body-color">{point}</p>
			{/each}
		</div>
	</div>
{/if}

<style>
	p {
		margin-bottom: 0.618rem;
	}
</style>