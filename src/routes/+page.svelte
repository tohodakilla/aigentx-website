<script>
	import hero from '$lib/images/hero.jpg'
	import robot from '$lib/images/robot.webp'
	import Icon from '@iconify/svelte'

	import Menu from '../lib/Menu.svelte'
	import Roadmap from '../lib/Roadmap.svelte'
	import RoadmapItem from '../lib/RoadmapItem.svelte'
	import Tokenomics from '../lib/Tokenomics.svelte'
	import Testimonials from '../lib/Testimonials.svelte'
</script>

<Menu />

<div class="hero">
	<img class="hro" src={hero} alt="AIgentX">
	<img class="robot" src={robot} alt="AIgentX robot">
</div>

<section id="home" class="relative z-10 pt-16 pb-10">
	<div class="container">
	  <div class="-mx-4 flex flex-wrap">
		<div class="w-full px-4">
		  <div class="mx-auto max-w-[720px] text-center">
			<h1 class="mb-4 text-3xl font-bold leading-tight text-body-color dark:text-white md:text-[45px]">AIgentX: An innovative AI Ecosystem Enabling Improved Engagement and Project Oversight.</h1>
			<p class="mx-auto mb-4 max-w-[620px] text-lg font-medium text-body-color-2">AIgentX is a dynamic AI ecosystem that harnesses advanced AI and ML technologies. It utilizes custom business and project data to provide detailed, natural language responses, optimizing interactions, and reducing costs while offering comprehensive AI solutions for businesses and projects across platforms like Telegram and Discord. This ecosystem empowers users to create personalized AI for improved community engagement, accurate project represenation, customer satisfaction and sales growth.</p>
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

<section id="features">
	<div class="mx-auto mb-20">
		<div class="container">
			<div class="text-center">
				<p class="text-2xl mb-6"><span class="font-bold">🤖 Personalized Moderation:</span> AigentX, your chat moderator, maintains respect, responds 24/7.</p>
				<p class="text-2xl mb-6"><span class="font-bold">📊 Custom Insights:</span> Get tailor-made community insights, manage queries, align with your project's identity.</p>
				<p class="text-2xl mb-6"><span class="font-bold">🔗 Seamless Integration:</span> Blend AigentX into Discord and Telegram for unified community experiences.</p>
				<p class="text-2xl mb-6"><span class="font-bold">🛠️ Effortless Customization:</span> Easily adapt AigentX to your community's unique needs.</p>
				<p class="text-2xl mb-6"><span class="font-bold">👍 User-Friendly </span>Setup: Configure custom agents intuitively, align with community dynamics.</p>
				<p class="text-2xl mb-6"><span class="font-bold">🤝 Dedicated Support:</span> AigentX adapts to your community's context, portrays your project's identity.</p>
				<p class="text-2xl mb-6"><span class="font-bold">🧠 AI Excellence:</span> Harness NLP, ML, Automation for adaptable engagement.</p>
				<p class="text-2xl mb-6"><span class="font-bold">💰 SalesBotAI Integration:</span> Supercharge sales with instant responses, lead qualification.</p>
				<p class="text-2xl mb-6"><span class="font-bold">📈 Real-Time </span>Data: Stay informed with project data updates.</p>
				<p class="text-2xl mb-6"><span class="font-bold">🎯 Tailored Solutions:</span> AigentX customizes group chat, community engagement to match goals, identity.</p>
	
			</div>
		
		</div>
	
	</div>
</section>

<Tokenomics />

<div class="container pt-20 pb-10">
	<h2 class="text-3xl font-bold leading-tight text-white md:text-[45px] text-center lg:mb-9 mb-3">REVENUE SHARING</h2>
	<ul class="max-w-md	mx-auto">
		<li class="flex items-center justify-center gap-3 text-2xl mb-3 text-center"><svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 12 12"><path fill="#8ba6ff" d="M9.765 3.205a.75.75 0 0 1 .03 1.06l-4.25 4.5a.75.75 0 0 1-1.075.015L2.22 6.53a.75.75 0 0 1 1.06-1.06l1.705 1.704l3.72-3.939a.75.75 0 0 1 1.06-.03Z"/></svg>1% of all AIgentX trading volume</li>
		<li class="flex items-center justify-center gap-3 text-2xl mb-3 text-center"><svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 12 12"><path fill="#8ba6ff" d="M9.765 3.205a.75.75 0 0 1 .03 1.06l-4.25 4.5a.75.75 0 0 1-1.075.015L2.22 6.53a.75.75 0 0 1 1.06-1.06l1.705 1.704l3.72-3.939a.75.75 0 0 1 1.06-.03Z"/></svg>5% of all AigentX Revenue</li>
		<li class="flex items-center justify-center gap-3 text-2xl mb-3 text-center"><svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 12 12"><path fill="#8ba6ff" d="M9.765 3.205a.75.75 0 0 1 .03 1.06l-4.25 4.5a.75.75 0 0 1-1.075.015L2.22 6.53a.75.75 0 0 1 1.06-1.06l1.705 1.704l3.72-3.939a.75.75 0 0 1 1.06-.03Z"/></svg>20% affiliate marketing</li>
	</ul>
</div>


<div class="spacer"></div>


<Roadmap>
	<RoadmapItem
		side=left
		quarter="Q2 2023"
		points={[
			'SalesBotAI launch'
		]}
		done={[true]}
	/>
	<RoadmapItem
		side=right
		quarter="Q3 2023"
		points={[
			'Launched website showcasing offerings',
			'Completed crypto-focused demo bot',
			'Initiated key partnerships',
			'Deployed custom chat bots for Telegram',
			'Initial development of AIgentX',
			'Deploy custom chat bots for telegram'
		]}
		done={[true, true, true, true, true, true]}
	/>
	<RoadmapItem
		side=left
		quarter="Q4 2023"
		points={[
			'Develop web-based UI for custom chat bots',
			'Enhance website and branding',
			'Form strategic partnerships',
			'CoinMarketCap + CoinGecko listing',
			'Implement advanced revenue sharing model',
			'Launch affiliate program for token holders'
		]}
		done={[]}
	/>
	<RoadmapItem
		side=right
		quarter="Q1 2024"
		points={[
			'Commence integration of advanced chat bot tools such as signal bots',
			'Develop a custom chat bot trading suite for enhanced functionality'
		]}
		done={[]}
	/>
</Roadmap>

<Testimonials />

<section id="footer" class="pt-16 pb-10">
	<div class="container">
		<div class="flex mb-6 gap-6 justify-center">
			<p class="text-body-color flex items-center"><a href="https://twitter.com/aigentx0x"><Icon icon=line-md:twitter-x-alt style="font-size:32px" /></a></p>
			<p class="text-body-color flex items-center"><a href="https://telegram.com"><Icon icon=ph:telegram-logo-duotone style="font-size:32px" /></a></p>
			<p class="text-body-color flex items-center"><a href="https://medium.com"><Icon icon=mdi:medium style="font-size:32px" /></a></p>
		</div>
		<p class="text-center text-body-color-2">copyright AIgentX 2023</p>
	</div>
</section>

<style>
	:global(html) {
		scroll-behavior: smooth;
	}
	:global(html,body) {
		background: #000225;
		color: #fff;
	}
	.hero {
		padding-top: 69px;
	}
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
	.hro {
		display: block
	}
	.robot {
		display: none;
	}
	@media only screen and (max-width: 767px) {
		.hro { display: none }
		.robot {
			display: block;
		}
	}
</style>