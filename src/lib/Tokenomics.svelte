<script>
	import { reveal } from 'svelte-reveal'
	import { onMount } from 'svelte'

	let ApexCharts

	onMount(async () => {
		ApexCharts = (await import('apexcharts')).default
		const charts = document.querySelectorAll('#chart');
		if(charts.length) {
			let options = {
				series: [100],
				chart: { type: 'donut', width: 400 },
				colors: ["#2347B9", "#3363FF", "#8BA6FF", "#8696CA"],
				legend: { show: false },
				stroke: { show: false },
				responsive: [
					{
						breakpoint: 480,
						options: {
							chart: { width: 200 },
							legend: {
								position: 'bottom',
							},
						},
					},
				],
			}
  
			const chart = new ApexCharts(document.querySelector('#chart'), options)
			chart.render()
		}
	})
</script>

<section id="tokenomics" class="relative z-10">
	<div class="container">
		<div class="rounded-lg py-6 lg:py-12 lg:px-8 bg-[#14102C] sm:py-6 sm:px-3 lg:px-8 xl:px-14">
			<h2 class="text-3xl font-bold leading-tight text-white md:text-[45px] text-center lg:mb-9 mb-3">TOKENOMICS</h2>


			<div class="mx-4 flex flex-wrap items-center text-center lg:text-left">
				<div class="w-full px-4 lg:w-1/2 mb-6 lg:mb-0 lg:pl-28">
					<p class="text-left text-lg font-bold text-body-color">Token Name: <span class="font-medium">AIgentX</span></p>
					<p class="text-left text-lg font-bold text-body-color">Ticker: <span class="font-medium">AIX</span></p>
					<p class="text-left text-lg font-bold text-body-color">Max supply: <span class="font-medium">100,000,000</span></p>
					<p class="text-left text-lg font-bold text-body-color">Network: <span class="font-medium">ETH (ERC-20)</span></p>
					<div class="mt-6">
						<p class="flex mb-1.5">
							<span class="mr-4 h-6 w-6 rounded-full bg-primary"></span>
							<span class="text-lg font-medium text-body-color"><strong>100% Stealth launch</strong></span>
						</p>
						<p class="flex mb-1.5">
							<span class="mr-4 h-6 w-6 rounded-full bg-[#2347B9]"></span>
							<span class="text-lg font-medium text-body-color">5% Buy tax</span>
						</p>
						<p class="flex mb-1.5">
							<span class="mr-4 h-6 w-6 rounded-full bg-[#8BA6FF]"></span>
							<span class="text-lg font-medium text-body-color">5% Sell tax</span>
						</p>
					</div>
				</div>

				<div class="w-full px-4 lg:w-1/2">
					<div class="mb-12 flex items-center justify-center lg:mb-0" use:reveal={{ delay: 0 }}>
						<div id="chart"></div>
					</div>
				</div>
				<div class="text-center w-full mt-6">
					<p class="text-center text-xl mb-3 w-full"><span class="font-bold">token address:</span>0x3fdfd866fa9e1ab4b6f6762cbdce0bf787583dc3</p>
					<p class="text-center text-xl mb-3 w-full"><a class="font-bold underline" href="https://dexscreener.com/ethereum/0x3fdfd866fa9e1ab4b6f6762cbdce0bf787583dc3" target="_blank">dexscreener</a></p>
				</div>
				<div class="w-full mx-6">
					<p class="text-center text-xl mb-3 w-full">🚫 (No team tokens, No presale/private sale, 100% Pooled)</p>
					<p class="text-center text-xl">🔢 5% Buy and Sell taxes (📣 Marketing, 🤝 Partnership, 💻 Development, and 💵 Revenue Sharing)</p>

				</div>
			</div>
		</div>
	</div>

	<div class="absolute right-0 -top-32 -z-10">
		<img src="images/shapes/token-sale-shape.svg" alt="shape" />
	</div>
</section>

