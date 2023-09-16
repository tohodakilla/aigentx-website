<script>
	import Icon from '@iconify/svelte'
	import logo from '$lib/images/logo.png'
	import Modal from '../lib/Modal.svelte'

	let showModal = true
	let menuOpen
	let w

	const openModal = () => {
		// showModal = true
		// menuOpen = false
	}
</script>

<svelte:window bind:innerWidth={w} />

<nav>
	<div class="container h-full">
		<div class="flex items-center justify-between h-full relative">
			<a href="/"><img class="logo" src={logo} alt="AIgentX logo"></a>

			{#if w < 1024}
				<button
					on:click={() => menuOpen = !menuOpen}
					class="block rounded-lg px-3 py-[6px] ring-primary focus:ring-2 xl:hidden"
					style="right: 0"
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
				<ul class="flex gap-6 font-semibold">
					<li class="text-body-color py-3"><a href="#tokenomics">tokenomics</a></li>
					<li class="text-body-color py-3"><a href="#roadmap">roadmap</a></li>
					<li class="text-body-color py-3"><a href="#features">features</a></li>
					<li class="text-body-color py-3"><a target="_blank" href="https://aigentx.gitbook.io/whitepaper/">whitepaper</a></li>
					<li class="text-body-color flex items-center"><a target="_blank" href="https://twitter.com/0xAIgentx"><Icon icon=line-md:twitter-x-alt style="font-size:32px" /></a></li>
					<li class="text-body-color flex items-center"><a target="_blank" href="https://t.me/+hWMgnOdPhG40Nzhl"><Icon icon=ph:telegram-logo-duotone style="font-size:32px" /></a></li>
					<!-- <li class="text-body-color flex items-center"><a href="https://medium.com"><Icon icon=mdi:medium style="font-size:32px" /></a></li> -->
					<li class="text-body-color flex items-center"><a target="_blank" href="mailto:0xaigentx@gmail.com"><Icon icon=material-symbols:alternate-email-rounded style="font-size:32px" /></a></li>
					<li class="text-body-color">
						<a
							target="_blank"
							href="https://app.uniswap.org/swap?outputCurrency=0x40e9187078032afe1a30cfcf76e4fe3d7ab5c6c5&chain=ethereum"
							class="block align-center rounded-full bg-primary text-lg text-white uppercase px-6 py-3 hover:bg-opacity-90 active:scale-95"
						>
							<span>buy now</span>
							<!-- <a href="https://uniswap.org">buy now</a> -->
						</a>
					</li>
				</ul>
			{/if}

			{#if menuOpen}
				<div class="absolute right-4 top-full w-full max-w-[250px] rounded-lg py-4 px-6 shadow bg-black lg:static lg:block lg:w-full lg:max-w-full lg:bg-transparent lg:py-0 lg:shadow-none">
					<ul class="w-full">
						<li class="text-body-color py-3"><a href="#tokenomics">tokenomics</a></li>
						<li class="text-body-color py-3"><a href="#roadmap">roadmap</a></li>
						<li class="text-body-color py-3"><a href="#features">features</a></li>
						<li class="text-body-color py-3"><a target="_blank" href="https://aigentx.gitbook.io/whitepaper/">whitepaper</a></li>
						<div class="flex mb-6">
							<li class="text-body-color flex items-center"><a target="_blank" href="https://twitter.com/0xAIgentx"><Icon icon=line-md:twitter-x-alt style="font-size:32px" /></a></li>
							<li class="text-body-color flex items-center"><a target="_blank" href="https://t.me/+hWMgnOdPhG40Nzhl"><Icon icon=ph:telegram-logo-duotone style="font-size:32px" /></a></li>
							<li class="text-body-color flex items-center"><a target="_blank" href="mailto:0xaigentx@gmail.com"><Icon icon=material-symbols:alternate-email-rounded style="font-size:32px" /></a></li>
							<!-- <li class="text-body-color flex items-center"><a href="https://medium.com"><Icon icon=mdi:medium style="font-size:32px" /></a></li> -->

						</div>
						<li class="text-body-color">
							<a
								target="_blank"
								href="https://app.uniswap.org/swap?outputCurrency=0x40e9187078032afe1a30cfcf76e4fe3d7ab5c6c5&chain=ethereum"
								class="block align-center rounded-full bg-primary text-lg text-white uppercase px-6 py-3 hover:bg-opacity-90 active:scale-95"
							>
								<span>buy now</span>
								<!-- <a href="https://uniswap.org">buy now</a> -->
							</a>
						</li>
					</ul>
				</div>
			{/if}
		</div>
	</div>
</nav>

<!-- <Modal bind:showModal>
	<div class="w-full">
		<div class="rounded-lg bg-dark py-12 px-8 sm:py-16 sm:px-14">
		  <div class="mb-24">
			<div class="flex items-start justify-center">
			  <div class="text-center">
				<span class="mb-2 block text-2xl font-bold text-white sm:text-3xl md:text-[45px]"> 616 </span>
				<span class="text-xs font-medium uppercase text-white sm:text-sm md:text-lg"> DAYS </span>
			  </div>
			  <span class="px-2 text-2xl font-bold text-white sm:px-4 sm:text-3xl md:text-[45px]"> : </span>
			  <div class="text-center">
				<span class="mb-2 block text-2xl font-bold text-white sm:text-3xl md:text-[45px]"> 0 </span>
				<span class="text-xs font-medium uppercase text-white sm:text-sm md:text-lg"> HOURS </span>
			  </div>
			  <span class="px-2 text-2xl font-bold text-white sm:px-4 sm:text-3xl md:text-[45px]"> : </span>
			  <div class="text-center">
				<span class="mb-2 block text-2xl font-bold text-white sm:text-3xl md:text-[45px]"> 45 </span>
				<span class="text-xs font-medium uppercase text-white sm:text-sm md:text-lg"> MINUTES </span>
			  </div>
			  <span class="px-2 text-2xl font-bold text-white sm:px-4 sm:text-3xl md:text-[45px]"> : </span>
			  <div class="text-center">
				<span class="mb-2 block text-2xl font-bold text-white sm:text-3xl md:text-[45px]"> 03 </span>
				<span class="text-xs font-medium uppercase text-white sm:text-sm md:text-lg"> SECONDS </span>
			  </div>
			</div>
		  </div>
		  <div class="mb-8">
			<div class="relative z-20">
			  <div class="relative h-8 w-full rounded-full bg-[#515A95]">
				<div class="absolute left-0 bottom-0 h-full w-[75%] rounded-full bg-primary"></div>
				<div class="absolute bottom-0 left-0 flex w-full justify-around">
				  <div class="group relative flex w-1/3 justify-center">
					<div class="h-9 w-[2px] bg-[#384280]"></div>
					<div class="absolute top-[-140%] left-1/2 z-20 -translate-x-1/2 whitespace-nowrap rounded-full bg-[#384280] px-5 py-2 text-sm font-semibold text-white opacity-0 group-hover:opacity-100">
					  <span class="absolute -bottom-1 left-1/2 h-3 w-3 -translate-x-1/2 rotate-45 bg-[#384280]"></span>
					  <span>PRE-SALE</span>
					</div>
				  </div>
				  <div class="group relative flex w-1/3 justify-center">
					<div class="h-9 w-[2px] bg-[#384280]"></div>
					<div class="absolute top-[-140%] left-1/2 z-20 -translate-x-1/2 whitespace-nowrap rounded-full bg-[#384280] px-5 py-2 text-sm font-semibold text-white opacity-0 group-hover:opacity-100">
					  <span class="absolute -bottom-1 left-1/2 h-3 w-3 -translate-x-1/2 rotate-45 bg-[#384280]"></span>
					  <span>SOFT CAP</span>
					</div>
				  </div>
				  <div class="group relative flex w-1/3 justify-center">
					<div class="h-9 w-[2px] bg-[#384280]"></div>
					<div class="absolute top-[-140%] left-1/2 z-20 -translate-x-1/2 whitespace-nowrap rounded-full bg-[#384280] px-5 py-2 text-sm font-semibold text-white opacity-0 group-hover:opacity-100">
					  <span class="absolute -bottom-1 left-1/2 h-3 w-3 -translate-x-1/2 rotate-45 bg-[#384280]"></span>
					  <span>BONUS</span>
					</div>
				  </div>
				</div>
			  </div>
			</div>
		  </div>
		  <div class="mb-10 text-center">
			<button class="rounded-full bg-primary py-3 px-8 text-base font-semibold text-white hover:bg-opacity-90"> Buy Token Now </button>
		  </div>
		  <div class="text-center">
			<img src="images/sale-token/payment-method.svg" alt="payment-method" class="mx-auto dark:grayscale-0" />
		  </div>
		</div>
	  </div>
</Modal> -->

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
					