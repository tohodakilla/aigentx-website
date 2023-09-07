<script>
	// import { onMount } from 'svelte'

	// let ApexCharts

	// onMount(async () => {
	// 	ApexCharts = (await import('apexcharts')).default
	// 	const charts = document.querySelectorAll('#chart');
	// 	if(charts.length) {
	// 		let options = {
	// 			series: [73, 55, 38, 20],
	// 			chart: { type: 'donut', width: 400 },
	// 			colors: ["#2347B9", "#3363FF", "#8BA6FF", "#8696CA"],
	// 			legend: { show: false },
	// 			stroke: { show: false },
	// 			responsive: [
	// 				{
	// 					breakpoint: 480,
	// 					options: {
	// 						chart: { width: 200 },
	// 						legend: {
	// 							position: 'bottom',
	// 						},
	// 					},
	// 				},
	// 			],
	// 		}
  
	// 		const chart = new ApexCharts(document.querySelector('#chart'), options)
	// 		chart.render()
	// 	}
	// })
</script>

<section class="relative z-10">
	<div class="container">
		<div class="rounded-lg py-12 px-8 bg-[#14102C] sm:py-16 sm:px-14 lg:px-8 xl:px-14">
			<h2 class="text-3xl font-bold leading-tight text-white md:text-[45px] text-center lg:mb-9">TOKENOMICS</h2>
			<div class="-mx-4 flex flex-wrap items-start">
				<div class="w-full px-4 lg:w-1/2 mb-6 lg:mb-0">
					<div class="wow fadeInUp mb-12 flex items-center justify-center lg:mb-0" data-wow-delay="0s">
						

					</div>
					<div>
						<p class="text-left text-lg font-bold text-body-color">Token Name: <span class="font-medium">AIgentX</span></p>
						<p class="text-left text-lg font-bold text-body-color">Ticker: <span class="font-medium">AIX</span></p>
						<p class="text-left text-lg font-bold text-body-color">Max supply: <span class="font-medium">100,000,000</span></p>
						<p class="text-left text-lg font-bold text-body-color">Network: <span class="font-medium">ETH (ERC-20)</span></p>
					</div>
				</div>

				<div class="w-full px-4 lg:w-1/2 text-center">
	
						<p class="flex mb-1.5">
							<span class="mr-4 h-6 w-6 rounded-full bg-primary"></span>
							<span class="text-lg font-medium text-body-color">100% Stealth launch</span>
						</p>
						<p class="flex mb-1.5">
							<span class="mr-4 h-6 w-6 rounded-full bg-[#2347B9]"></span>
							<span class="text-lg font-medium text-body-color">5% Buy tax</span>
						</p>
						<p class="flex mb-1.5">
							<span class="mr-4 h-6 w-6 rounded-full bg-[#8BA6FF]"></span>
							<span class="text-lg font-medium text-body-color">5% Sell tax</span>
						</p>
						<p class="flex mb-1.5">
							<span class="mr-4 h-6 w-6 rounded-full bg-[#8696CA]"></span>
							<span class="text-lg font-medium text-body-color text-left">1% revenue share<br>1% team<br>2% product dev, marketing<br>1% partnering</span>
						</p>
				</div>
			</div>
		</div>
	</div>

	<div class="absolute right-0 -top-32 -z-10">
		<img src="images/shapes/token-sale-shape.svg" alt="shape" />
	</div>
</section>

