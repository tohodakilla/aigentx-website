<script>
	import { onMount } from 'svelte'
	import hero from '$lib/images/hero.jpg'
	import Icon from '@iconify/svelte'

	import Roadmap from '../lib/Roadmap.svelte'
	import RoadmapItem from '../lib/RoadmapItem.svelte'
	import Tokenomics from '../lib/Tokenomics.svelte'
	import Testimonials from '../lib/Testimonials.svelte'
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
			<h1 class="mb-4 text-3xl font-bold leading-tight text-body-color dark:text-white md:text-[45px]">Revolutionize Your Telegram Groups with AigentX: Elevate Engagement and Boost Community Growth!</h1>
			<p class="mx-auto mb-4 max-w-[620px] text-lg font-medium text-body-color-2">AigentX leverages advanced technologies like Natural Language Processing and Machine Learning to revolutionize the Telegram group experience, providing a suite of features tailored for group chats, crypto project channels, and active community engagement. More than just a chatbot, it serves as your one-stop crypto assistant. AigentX empowers users with instant answers about cryptocurrency projects, real-time portfolio management, and more. It offers multi-platform compatibility, extending services to Discord, Facebook, and WhatsApp. Users can customize the bot's personality, response style, and knowledge base, and even upload content in various formats for the bot's learning. The system supports multiple bots across different channels for enhanced community engagement and is capable of fetching real-time project data from various sources. AigentX sets a new standard for Telegram-based crypto interactions, providing tailored excellence in customer relations, sales, and service.</p>
			<div class="py-3"></div>
			<button href="#features" class="rounded-full bg-primary py-5 px-16 text-lg font-semibold text-white hover:bg-opacity-90 active:scale-95">TRY IT OUT</button>
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


<Tokenomics />

<Roadmap>
	<RoadmapItem
		side=left
		quarter="Q2 2023 Achievements:"
		points={[
			'Launched initial product, paving the way for development.',
			'Deployed SalesBotAI, boosting sales and interactions.',
			'First partnerships'
		]}
	/>
	<RoadmapItem
		side=right
		quarter="Q3 2023 Achievements:"
		points={[
			'Launched website showcasing offerings.',
			'Completed crypto-focused demo bot.',
			'Initiated key partnerships.',
			'Deployed custom chat bots for Telegram.'
		]}
	/>
	<RoadmapItem
		side=left
		quarter="Q4 2023 Objectives:"
		points={[
			'Develop web-based UI for custom chat bots.',
			'Enhance website and branding.',
			'Form strategic partnerships.',
			'CoinMarketCap + CoinGecko listing',
			'Implement revenue sharing and advanced models.',
			'Launch affiliate program for tokenholders.'
		]}
	/>
	<RoadmapItem
		side=right
		quarter="Q1 2024 Objectives:"
		points={[
			'Commence integration of advanced chat bot tools such as signal bots.',
			'Develop a custom chat bot trading suite for enhanced functionality.'
		]}
	/>
</Roadmap>

<Testimonials />


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