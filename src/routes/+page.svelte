<script>
	import { onMount } from 'svelte'
	import hero from '$lib/images/hero.jpg'
	import Icon from '@iconify/svelte'
	
	let ApexCharts

	onMount(async () => {
		ApexCharts = (await import('apexcharts')).default
		const charts = document.querySelectorAll('#chart');
if(charts.length) {
  let options = {
    series: [73, 55, 38, 20],
    chart: {
      type: "donut",
      width: 400,
    },
    colors: ["#2347B9", "#3363FF", "#8BA6FF", "#8696CA"],
    legend: {
      show: false,
    },
    stroke: {
      show: false,
    },
    responsive: [
      {
        breakpoint: 480,
        options: {
          chart: {
            width: 200,
          },
          legend: {
            position: "bottom",
          },
        },
      },
    ],
  };
  
  const chart = new ApexCharts(document.querySelector("#chart"), options);
  chart.render();
}

	})
</script>

<!-- <header>
	<ul>
		<li class="text-body-color">
			<a href="#home"
				class="scroll-menu flex py-2 text-lg font-semibold text-primary hover:text-primary dark:text-white dark:hover:text-white lg:ml-7 lg:inline-flex lg:py-5 xl:ml-10 2xl:ml-12"
			>HOME</a>
		</li>
		<li class="text-body-color">
			<a href="#home"
				class="scroll-menu flex py-2 text-lg font-semibold text-primary hover:text-primary dark:text-white dark:hover:text-white lg:ml-7 lg:inline-flex lg:py-5 xl:ml-10 2xl:ml-12"
			>FEATURES</a>
		</li>
		<li class="text-body-color">
			<a href="#home"
				class="scroll-menu flex py-2 text-lg font-semibold text-primary hover:text-primary dark:text-white dark:hover:text-white lg:ml-7 lg:inline-flex lg:py-5 xl:ml-10 2xl:ml-12"
			>ROADMAP</a>
		</li>
		<li class="text-body-color">
			<a href="#home"
				class="scroll-menu flex py-2 text-lg font-semibold text-primary hover:text-primary dark:text-white dark:hover:text-white lg:ml-7 lg:inline-flex lg:py-5 xl:ml-10 2xl:ml-12"
			>TOKENOMICS</a>
		</li>
		<li class="text-body-color">
			<a href="#home"
				class="scroll-menu flex py-2 text-lg font-semibold text-primary hover:text-primary dark:text-white dark:hover:text-white lg:ml-7 lg:inline-flex lg:py-5 xl:ml-10 2xl:ml-12"
			>TELEGRAM</a>
		</li>
	</ul>
</header> -->

<div class="hero">
	<img src={hero} alt="AIgentX">
</div>

<section id="home" class="relative z-10 pt-16 pb-10">
	<div class="container">
	  <div class="-mx-4 flex flex-wrap">
		<div class="w-full px-4">
		  <div class="mx-auto max-w-[720px] text-center">
			<h1 class="mb-4 text-3xl font-bold leading-tight text-body-color dark:text-white md:text-[45px]">Meet AIgentX your versatile and comprehensive crypto assistant right on Telegram.</h1>
			<p class="mx-auto mb-4 max-w-[620px] text-lg font-medium text-body-color-2">Leveraging advanced technologies like Natural Language Processing and Machine Learning to provide a suite of features including a cryptocurrency-focused AI for handling inquiries, summarizing conversations, and detecting scams. It offers multi-platform compatibility, extending its services to Discord, Facebook, and WhatsApp. Users can customize the bot's personality, response style, and knowledge base, and even upload content in various formats for the bot's learning. The system supports multiple bots across different channels for enhanced community engagement and is capable of fetching real-time project data from multiple sources.</p>
			<div class="py-3"></div>
			<button href="#somewhere" class="rounded-full bg-primary py-5 px-16 text-lg font-semibold text-white hover:bg-opacity-90 active:scale-95">TRY IT OUT</button>
		  </div>
		</div>
	  </div>
	</div>
	<div class="absolute top-0 left-0 -z-10 h-full w-full opacity-20" style="background-image: linear-gradient(rgb(62, 125, 255) 0%, rgba(62, 125, 255, 0) 100%)"></div>
	<!-- <img src="images/shapes/hero-shape-1.svg" alt="" class="absolute left-0 top-0 -z-10"> -->
	<img src="images/shapes/hero-shape-2.svg" alt="" class="absolute right-0 top-0 -z-10">
  </section>

<div class="spacer"></div>

  <section id="features" class="pt-20 pb-16">
	<div class="container">
		<div class="wow fadeInUp mx-auto mb-16 max-w-[590px] text-center md:mb-20" data-wow-delay="0s">
			<span class="mb-3 text-lg font-bold uppercase text-primary sm:text-xl">The All-in-One</span>
			<h2 class="mb-3 text-3xl font-bold leading-tight text-white md:text-[45px]">Customizable Crypto Assistant for Your Business</h2>
			<!-- <p class="text-lg font-medium text-body-color"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc sed congue arcu, In et dignissim quam condimentum vel. </p> -->
		</div>
		<div class="-mx-4 flex flex-wrap">
			<div class="w-full px-4 md:w-1/2 lg:w-1/3">
				<div class="wow fadeInUp mx-auto mb-14 max-w-[370px] text-center" data-wow-delay="0s">
					<div class="mx-auto mb-7 flex h-20 w-20 items-center justify-center rounded-full bg-primary text-white">
						<Icon icon=material-symbols:inbox-customize-rounded style="font-size:42px;color:white;"/>
					</div>
					<div>
						<h3 class="mb-3 text-xl font-bold text-white sm:text-3xl lg:text-xl xl:text-3xl">Customization Like Never Before</h3>
						<p class="text-base font-medium text-body-color sm:text-lg lg:text-base xl:text-lg">Tailor the chatbot to your specific project's needs. Choose from custom data sources including YouTube, PDFs, web pages, voice notes, and chat logs for a truly personalized experience.</p>
					</div>
				</div>
			</div>
			<div class="w-full px-4 md:w-1/2 lg:w-1/3">
				<div class="wow fadeInUp mx-auto mb-14 max-w-[370px] text-center" data-wow-delay="0s">
					<div class="mx-auto mb-7 flex h-20 w-20 items-center justify-center rounded-full bg-primary text-white">
						<Icon icon=icon-park-twotone:sales-report style="font-size:42px;color:white;"/>
					</div>
					<div>
						<h3 class="mb-3 text-xl font-bold text-white sm:text-3xl lg:text-xl xl:text-3xl">Integrated with SalesbotAI</h3>
						<p class="text-base font-medium text-body-color sm:text-lg lg:text-base xl:text-lg">AigentX joins forces with SalesbotAI, ensuring rapid responses and meaningful engagements that translate to better business results.</p>
					</div>
				</div>
			</div>
			<div class="w-full px-4 md:w-1/2 lg:w-1/3">
				<div class="wow fadeInUp mx-auto mb-14 max-w-[370px] text-center" data-wow-delay="0s">
					<div class="mx-auto mb-7 flex h-20 w-20 items-center justify-center rounded-full bg-primary text-white">
						<Icon icon=streamline:interface-security-shield-3-shield-pay-product-secure-money-cash-currency-security-business style="font-size:42px;color:white;"/>
					</div>
					<div>
						<h3 class="mb-3 text-xl font-bold text-white sm:text-3xl lg:text-xl xl:text-3xl">Smart Business Integration</h3>
						<p class="text-base font-medium text-body-color sm:text-lg lg:text-base xl:text-lg">Use your existing business data like documents, presentations, and websites to enable AigentX to fully understand your services and style.</p>
					</div>
				</div>
			</div>
			<div class="w-full px-4 md:w-1/2 lg:w-1/3">
				<div class="wow fadeInUp mx-auto mb-14 max-w-[370px] text-center" data-wow-delay="0s">
					<div class="mx-auto mb-7 flex h-20 w-20 items-center justify-center rounded-full bg-primary text-white">
						<Icon icon=material-symbols:compare-arrows-rounded style="font-size:42px;color:white;"/>
					</div>
					<div>
						<h3 class="mb-3 text-xl font-bold text-white sm:text-3xl lg:text-xl xl:text-3xl">Wide Platform Compatibility</h3>
						<p class="text-base font-medium text-body-color sm:text-lg lg:text-base xl:text-lg"> Integrate seamlessly with Instagram, Facebook, Telegram, WhatsApp, Amo CRM, and more. Custom integrations also available upon request.</p>
					</div>
				</div>
			</div>
			<div class="w-full px-4 md:w-1/2 lg:w-1/3">
				<div class="wow fadeInUp mx-auto mb-14 max-w-[370px] text-center" data-wow-delay="0s">
					<div class="mx-auto mb-7 flex h-20 w-20 items-center justify-center rounded-full bg-primary text-white">
						<Icon icon=ion:language style="font-size:42px;color:white;"/>
					</div>
					<div>
						<h3 class="mb-3 text-xl font-bold text-white sm:text-3xl lg:text-xl xl:text-3xl">Speak Their Language</h3>
						<p class="text-base font-medium text-body-color sm:text-lg lg:text-base xl:text-lg">Communicate effortlessly in over 100 languages to cater to a global customer base.</p>
					</div>
				</div>
			</div>
			<div class="w-full px-4 md:w-1/2 lg:w-1/3">
				<div class="wow fadeInUp mx-auto mb-14 max-w-[370px] text-center" data-wow-delay="0s">
					<div class="mx-auto mb-7 flex h-20 w-20 items-center justify-center rounded-full bg-primary text-white">
						<Icon icon=streamline:money-cash-search-dollar-search-pay-product-currency-query-magnifying-cash-business-money-glass style="font-size:42px;color:white;"/>
					</div>
					<div>
						<h3 class="mb-3 text-xl font-bold text-white sm:text-3xl lg:text-xl xl:text-3xl">Cost-Efficient and Scalable</h3>
						<p class="text-base font-medium text-body-color sm:text-lg lg:text-base xl:text-lg">  Ideal for businesses of any size, AigentX services thousands of customers simultaneously, helping you save on personnel costs.</p>
					</div>
				</div>
			</div>
		</div>
	</div>
</section>

<section class="relative z-10">
	<div class="container">
		<div class="rounded-lg py-12 px-8 bg-[#14102C] sm:py-16 sm:px-14 lg:px-8 xl:px-14">
			<div class="-mx-4 flex flex-wrap items-center">
				<div class="w-full px-4 lg:w-1/2">
					<div class="wow fadeInUp mb-12 flex items-center justify-center lg:mb-0" data-wow-delay="0s">
						<div id="chart"></div>
					</div>
				</div>

				<div class="w-full px-4 lg:w-1/2">
					<div class="wow fadeInUp mb-9" data-wow-delay="0s">
						<!-- <span class="mb-3 text-lg font-bold uppercase text-primary sm:text-xl">TOKENOMICS</span> -->
						<h2 class="mb-3 text-3xl font-bold leading-tight text-white md:text-[45px]">TOKENOMICS</h2>
						<p class="text-lg font-medium text-body-color">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus condimentum tellus at lectus pulvinar, id auctor felis iaculis. In vestibulum neque sem, at dapibus justo facilisis in.</p>
					</div>
	
					<div class="wow fadeInUp space-y-4" data-wow-delay="0s">
						<p class="flex">
							<span class="mr-4 h-6 w-6 rounded-full bg-primary"></span>
							<span class="text-lg font-medium text-body-color">73% Financial Overhead</span>
						</p>
						<p class="flex">
							<span class="mr-4 h-6 w-6 rounded-full bg-[#2347B9]"></span>
							<span class="text-lg font-medium text-body-color">55% Bonus & found</span>
						</p>
						<p class="flex">
							<span class="mr-4 h-6 w-6 rounded-full bg-[#8BA6FF]"></span>
							<span class="text-lg font-medium text-body-color">38% it infastrueture</span>
						</p>
						<p class="flex">
							<span class="mr-4 h-6 w-6 rounded-full bg-[#8696CA]"></span>
							<span class="text-lg font-medium text-body-color">20.93% Gift Code Inventory</span>
						</p>
					</div>
				</div>
			</div>
		</div>
	</div>

	<div class="absolute right-0 -top-32 -z-10">
		<img src="images/shapes/token-sale-shape.svg" alt="shape" />
	</div>
</section>


<section id="roadmap" class="relative z-10 py-[120px]">
	<div class="container">
		<div class="wow fadeInUp mx-auto mb-16 max-w-[590px] text-center md:mb-20" data-wow-delay="0s">
			<span class="mb-3 text-lg font-bold uppercase text-primary sm:text-xl"> ROADMAP </span>
			<h2 class="mb-3 text-3xl font-bold leading-tight text-white md:text-[45px]"> The Timeline </h2>
			<p class="text-lg font-medium text-body-color"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc sed congue arcu, In et dignissim quam condimentum vel. </p>
		</div>

		<div class="-mx-4 flex justify-center">
			<div class="w-full px-4 lg:w-10/12 xl:w-9/12">
				<div class="wow fadeInUp relative -mx-4 flex flex-wrap md:py-14 lg:py-20" data-wow-delay="0s">
					<span class="absolute top-0 left-2 hidden h-full w-[2px] bg-[#2D2C4A] md:left-1/2 md:block"></span>

				<div class="w-full px-4 md:w-1/2">
					<div class="relative z-10 mb-10 rounded-lg py-8 px-6 bg-dark md:mr-3 md:mb-0 md:text-right lg:mr-5">
						<span class="absolute top-1/2 left-0 hidden h-4 w-4 -translate-y-1/2 rounded-full border-4 bg-white border-body-color md:left-auto md:-right-9 md:block lg:-right-11"></span>
						<span class="absolute -right-1 top-1/2 hidden h-3 w-3 -translate-y-1/2 rotate-45 bg-dark md:block"></span>
						<h3 class="mb-3 text-xl font-bold text-white">Q4 2023</h3>
						<p class="text-base font-medium text-body-color">
							Full integration of AigentX and SalesbotAI<br>
							Launch of custom Telegram bot setup service<br>
							Seed round for early investors<br>
							Stealth Token launch<br>
							Marketing campaigns
						</p>
					</div>
				</div>

				<div class="w-full px-4 md:w-1/2"></div>
					<div class="w-full px-4 md:w-1/2"></div>
						<div class="w-full px-4 md:w-1/2">
							<div class="relative z-10 mb-10 rounded-lg py-8 px-6 bg-dark md:ml-3 md:mb-0 lg:ml-5">
<span class="absolute top-1/2 left-0 hidden h-4 w-4 -translate-y-1/2 rounded-full border-4 bg-white border-body-color md:right-auto md:-left-9 md:block lg:-left-11"></span>
<span class="absolute -left-1 top-1/2 hidden h-3 w-3 -translate-y-1/2 rotate-45 bg-dark md:block"></span>
<h3 class="mb-3 text-xl font-bold text-white">Late Q4 2023</h3>
<p class="text-base font-medium text-body-color">
	Advanced chatbot features<br>
    Partnerships for token/market analytics<br>
    Custom analytical data feeds, API integrations, news, and signals<br>
    Launch of custom chatbot trading suite
</p>

</div>
</div>
<!-- <div class="w-full px-4 md:w-1/2">
<div class="relative z-10 mb-10 rounded-lg py-8 px-6 bg-dark md:mr-3 md:mb-0 md:text-right lg:mr-5">
<span class="absolute top-1/2 left-0 hidden h-4 w-4 -translate-y-1/2 rounded-full border-4 bg-white border-body-color md:left-auto md:-right-9 md:block lg:-right-11"></span>
<span class="absolute -right-1 top-1/2 hidden h-3 w-3 -translate-y-1/2 rotate-45 bg-dark md:block"></span>
<h3 class="mb-3 text-xl font-bold text-white"> Mar 30,2021 </h3>
<p class="mb-5 text-base font-medium text-body-color"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc sed congue arcu, In et dignissim quam condimentum vel </p>
<a href="" class="inline-flex items-center justify-center rounded-full bg-white p-2 pr-3">
<span class="pr-1">
svg
</span>
<span class="pr-2 text-xs font-semibold text-body-color"> chainlink </span>
<span class="text-[8px] font-semibold text-[#959595]"> 4.5% </span>
<span>
svg
</span>
</a>
</div>
</div>
<div class="w-full px-4 md:w-1/2"></div>
<div class="w-full px-4 md:w-1/2"></div>
<div class="w-full px-4 md:w-1/2">
<div class="relative z-10 mb-10 rounded-lg py-8 px-6 bg-dark md:ml-3 md:mb-0 lg:ml-5">
<span class="absolute top-1/2 left-0 hidden h-4 w-4 -translate-y-1/2 rounded-full border-4 bg-white border-body-color md:right-auto md:-left-9 md:block lg:-left-11"></span>
<span class="absolute -left-1 top-1/2 hidden h-3 w-3 -translate-y-1/2 rotate-45 bg-dark md:block"></span>
<h3 class="mb-3 text-xl font-bold text-white"> Dec 19,2021 </h3>
<p class="mb-5 text-base font-medium text-body-color"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc sed congue arcu, In et dignissim quam condimentum vel </p>
<a href="" class="inline-flex items-center justify-center rounded-full bg-white p-2 pr-3">
<span class="pr-1">
svg
</span>
<span class="pr-2 text-xs font-semibold text-body-color"> polygon </span>
<span class="text-[8px] font-semibold text-[#959595]"> 2.5% </span>
<span>
svg
</span>
</a>
</div>
</div>
</div>
</div>
</div> -->
</div>
<div class="absolute left-0 bottom-0 -z-10">
<img src="images/shapes/timeline.svg" alt="shape" />
</div>
</section>


<style>
	:global(html,body) {
		background: #000225;
		color: #fff;
	}
	/* header ul {
		display: flex;
		justify-content: flex-end;

	} */
	/* header ul li {

	} */
	.hero img {
		width: 100%;
		border-bottom: 1px solid #141d6294;
	}
	button {
		transition: all 169ms cubic-bezier(0.23, 1, 0.32, 1)
	}
	.spacer {
		width: 80%;
		background: #2D2C4A;
		height: 1px;
		margin: 0 auto;
	}
</style>