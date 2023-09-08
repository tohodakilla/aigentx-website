<script>
	import Icon from '@iconify/svelte'
	import logo from '$lib/images/logo.png'

	let menuOpen
	let w
</script>

<svelte:window bind:innerWidth={w} />

<nav>
	<div class="container h-full">
		<div class="flex items-center justify-between h-full relative">
			<img class="logo" src={logo} alt="AIgentX logo">

			{#if w < 1024}
				<button
					on:click={() => menuOpen = !menuOpen}
					class="block rounded-lg px-3 py-[6px] ring-primary focus:ring-2 lg:hidden"
					class:menuOpen

				>
					<span
						class:relative={menuOpen}
						class:rotate-45={menuOpen}
						class:top-[7px]={menuOpen}
						class="relative my-[6px] block h-[2px] w-[30px] bg-white"
					></span>
					<span
						class:relative={menuOpen}
						class:opacity-0={menuOpen}
						class="relative my-[6px] block h-[2px] w-[30px] bg-white"
					></span>
					<span
						class:relative={menuOpen}
						class:top-[-8px]={menuOpen}
						class:rotate-[135deg]={menuOpen}
						class="relative my-[6px] block h-[2px] w-[30px] bg-white"
					></span>
				</button>

			{:else}
				<ul class="flex gap-6 font-semibold hover:">
					<li class="text-body-color py-3"><a href="#tokenomics">tokenomics</a></li>
					<li class="text-body-color py-3"><a href="#roadmap">roadmap</a></li>
					<li class="text-body-color py-3"><a href="#features">features</a></li>
					
					<li class="text-body-color flex items-center"><a href="https://twitter.com/aigentx0x"><Icon icon=line-md:twitter-x-alt style="font-size:32px" /></a></li>
					<li class="text-body-color flex items-center"><a href="https://telegram.com"><Icon icon=ph:telegram-logo-duotone style="font-size:32px" /></a></li>
					<li class="text-body-color flex items-center"><a href="https://medium.com"><Icon icon=mdi:medium style="font-size:32px" /></a></li>
					<li class="text-body-color">
						<button class="rounded-full bg-primary text-lg text-white uppercase px-6 py-3 hover:bg-opacity-90 active:scale-95">
							<a href="https://uniswap.org">buy now</a>
						</button>
					</li>
				</ul>
			{/if}

			{#if menuOpen}
				<div class="absolute right-4 top-full w-full max-w-[250px] rounded-lg py-4 px-6 shadow bg-black lg:static lg:block lg:w-full lg:max-w-full lg:bg-transparent lg:py-0 lg:shadow-none">
					<ul class="w-full">
						<li class="text-body-color py-3"><a href="#tokenomics">tokenomics</a></li>
						<li class="text-body-color py-3"><a href="#roadmap">roadmap</a></li>
						<li class="text-body-color py-3"><a href="#features">features</a></li>
						<div class="flex mb-6">
							<li class="text-body-color flex items-center"><a href="https://twitter.com/aigentx0x"><Icon icon=line-md:twitter-x-alt style="font-size:32px" /></a></li>
							<li class="text-body-color flex items-center"><a href="https://telegram.com"><Icon icon=ph:telegram-logo-duotone style="font-size:32px" /></a></li>
							<li class="text-body-color flex items-center"><a href="https://medium.com"><Icon icon=mdi:medium style="font-size:32px" /></a></li>

						</div>
						<li class="text-body-color">
							<button class="rounded-full bg-primary text-lg text-white uppercase px-6 py-3 hover:bg-opacity-90 active:scale-95">
								<a href="https://uniswap.org">buy now</a>
							</button>
						</li>
					</ul>
				</div>
			{/if}
		</div>
	</div>
</nav>

<style>
	nav {
		position: fixed;
		z-index: 100;
		width: 100%;
		background: transparent;
		backdrop-filter: blur(9px);
		/* background: linear-gradient(to right, #010229, #000326, #010229); */
		height: 69px;
	}
	nav .logo {
		height: 35px
	}
	li {
		font-size: 110%;
		text-transform: uppercase;

	}

	@media only screen and (max-width: 1023px) {
		span {
			transition: all 169ms cubic-bezier(0.23, 1, 0.32, 1);
		}
	}
</style>