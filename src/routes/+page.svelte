<script>
	import { reveal } from 'svelte-reveal'
	import hero from '$lib/images/hero_powered.webp'
	import robot from '$lib/images/robot_powered.webp'
	import Icon from '@iconify/svelte'

	import Access from '../lib/Access.svelte'
	import Cards from '../lib/Cards.svelte'
	import Menu from '../lib/Menu.svelte'
	import Roadmap from '../lib/Roadmap.svelte'
	import Success from '../lib/Success.svelte'
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
	<div class="container" use:reveal={{ delay: 0 }}>
	  <div class="-mx-4 flex flex-wrap">
		<div class="w-full px-4">
		  <div class="mx-auto max-w-[720px] text-center">
			<h1 class="mb-4 text-3xl font-bold leading-tight text-body-color dark:text-white md:text-[45px]">AIgentX: An innovative AI Ecosystem Enabling Improved Engagement and Project Oversight.</h1>
			<p class="mx-auto mb-4 max-w-[620px] text-lg font-medium text-body-color-2">AIgentX is a dynamic AI ecosystem that harnesses advanced AI and ML technologies. It utilizes custom business and project data to provide detailed, natural language responses, optimizing interactions, and reducing costs while offering comprehensive AI solutions for businesses and projects across platforms like Telegram and Discord. This ecosystem empowers users to create personalized AI for improved community engagement, accurate project represenation, customer satisfaction and sales growth.</p>
			<div class="py-3"></div>
			<a href="#try" class="rounded-full bg-primary py-5 px-16 text-lg font-semibold text-white hover:bg-opacity-90 active:scale-95">TRY IT OUT</a>
		  </div>
		</div>
	  </div>
	</div>
	<div class="absolute top-0 left-0 -z-10 h-full w-full opacity-20" style="background-image: linear-gradient(rgb(62, 125, 255) 0%, rgba(62, 125, 255, 0) 100%)"></div>
	<!-- <img src="images/shapes/hero-shape-1.svg" alt="" class="absolute left-0 top-0 -z-10"> -->
	<img src="images/shapes/hero-shape-2.svg" alt="" class="absolute right-0 top-0 -z-10">
</section>

<section id="features" class="bg-[#14102c] py-20">
	<div class="mx-auto mb-20">
		<div class="container">
			<h2 class="mb-3 text-3xl font-bold leading-tight text-white md:text-[45px] text-center">AIgentX transforms group interactions across multiple platforms, serving as a versatile crypto assistant setting a new crypto engagement standard</h2>
			<Cards feats={[
				{
				  emo: '🤖',
				  head: 'Personalized Moderation',
				  text: 'AigentX, your chat moderator, maintains respect, responds 24/7.'
				},
				{
				  emo: '📊',
				  head: 'Custom Insights',
				  text: "Get tailor-made community insights, manage queries, align with your project's identity."
				},
				{
				  emo: '🔗',
				  head: 'Seamless Integration',
				  text: 'Blend AigentX into Discord and Telegram for unified community experiences.'
				},
				{
				  emo: '🛠️',
				  head: 'Effortless Customization',
				  text: 'Easily adapt AigentX to your community\'s unique needs.'
				},
				{
				  emo: '👍',
				  head: 'User-Friendly Setup',
				  text: 'Configure custom agents intuitively, align with community dynamics.'
				},
				{
				  emo: '🤝',
				  head: 'Dedicated Support',
				  text: 'AigentX adapts to your community\'s context, portrays your project\'s identity.'
				},
				{
				  emo: '🧠',
				  head: 'AI Excellence',
				  text: 'Harness NLP, ML, Automation for adaptable engagement.'
				},
				{
				  emo: '📈',
				  head: 'Real-Time Data',
				  text: 'Stay informed with project data updates.'
				},
				{
				  emo: '🎯',
				  head: 'Tailored Solutions',
				  text: 'AigentX customizes group chat, community engagement to match goals, identity.'
				}
			  ]
			  } />
				
		</div>
	</div>
</section>

<section class="pt-20 bg-16">
	<div class="container">
		<div class="mx-auto mb-10 max-w-[590px] text-center md:mb-16" use:reveal={{ delay: 0 }}>
			<span class="mb-3 text-lg font-bold uppercase text-primary sm:text-xl">Integratly AI</span>
			<h2 class="mb-3 text-3xl font-bold leading-tight text-white md:text-[45px]">AIgentX Partners with Integratly AI: A Game-Changing Collaboration</h2>
		</div>

		<div class="-mx-4 flex flex-wrap" use:reveal={{ delay: 10 }}>
			<div class="w-full px-4">
			  <div class="mx-auto max-w-[720px] text-center">
				
				<p class="mx-auto mb-4 max-w-[620px] text-lg font-medium text-body-color-2">We're thrilled to announce our technical partnership with <a href="https://integratly.ai/" target="_blank">IntegratlyAI</a>, a leading authority in the custom AI solutions space. <a href="https://integratly.ai/" target="_blank">IntegratlyAI</a> boasts over a decade of expertise in AI and IT, offering specialized services designed for seamless business integration. They stand out for their commitment to high ROI and 100% guaranteed successful integration, making AI adoption easier and more efficient for businesses of all sizes. This collaboration aims to amplify both companies' strengths, combining AIgentX's focus on community engagement and project oversight with IntegratlyAI's proven, ROI-driven AI solutions.</p>

				<div class="pb-6"></div>
			  </div>
			</div>
		  </div>
	</div>
</section>

<div class="spacer"></div>

<Access />

<div class="spacer"></div>

<Success items={[{
	head: 'Baby BNB Tiger Bot on Telegram',
	text: 'We partnered with Integratly AI to create a specialized Telegram bot for the Baby BNB Tiger project. The results speak for themselves: heightened community engagement and a boost in token promotion.',
	link: 'http://t.me/Baby_BNB_Tiger_bot',
	button: 'Experience Baby BNB Tiger Bot',
	img: 'tiger'
},{
	head: 'Airdrop Hunter',
	text: `Integratly AI's platform transformed the cryptocurrency airdrop experience. With an intuitive interface and streamlined processes, we witnessed an exponential increase in user participation and engagement.`,
	link: 'https://airdrop-hunter.site/',
	button: 'Explore Airdrop Hunter Platform',
	img: 'airdrop'
},
// {
// 	head: 'Welcome To Bali Bot on Telegram',
// 	text: `Demonstrating the versatility of Integratly AI's solutions, we ventured beyond the crypto realm. The Welcome To Bali Bot on Telegram offers invaluable tourism-related information and services, expanding our reach to new horizons.`,
// 	link: 'https://t.me/WelcomeToBali_bot',
// 	button: 'Discover Welcome To Bali Bot',
// 	img: 'bali'
// },
{
	head: 'Narfex AI Bot on Telegram',
	text: 'Our partnership with Integratly AI brought advanced community management and user engagement to the forefront. Thanks to cutting-edge AI technology, we experienced unparalleled growth and efficiency in our community interactions.',
	link: 'https://t.me/NarfexAI_bot',
	button: 'Engage with Narfex AI Bot',
	img: 'narfex'
}]}/>

<div class="spacer"></div>

<div class="container pt-20 pb-10">
	<h2 class="text-3xl font-bold leading-tight text-white md:text-[45px] text-center lg:mb-9 mb-3">REVENUE SHARING</h2>
	<ul class="max-w-md	mx-auto">
		<li class="flex items-center justify-center gap-3 text-2xl mb-3 text-center"><svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 12 12"><path fill="#8ba6ff" d="M9.765 3.205a.75.75 0 0 1 .03 1.06l-4.25 4.5a.75.75 0 0 1-1.075.015L2.22 6.53a.75.75 0 0 1 1.06-1.06l1.705 1.704l3.72-3.939a.75.75 0 0 1 1.06-.03Z"/></svg><span>2% of all AIgentX trading volume</span></li>
		<li class="flex items-center justify-center gap-3 text-2xl mb-3 text-center"><svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 12 12"><path fill="#8ba6ff" d="M9.765 3.205a.75.75 0 0 1 .03 1.06l-4.25 4.5a.75.75 0 0 1-1.075.015L2.22 6.53a.75.75 0 0 1 1.06-1.06l1.705 1.704l3.72-3.939a.75.75 0 0 1 1.06-.03Z"/></svg><span>10% of all AigentX Revenue</span></li>
		<li class="flex items-center justify-center gap-3 text-2xl mb-3 text-center"><svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 12 12"><path fill="#8ba6ff" d="M9.765 3.205a.75.75 0 0 1 .03 1.06l-4.25 4.5a.75.75 0 0 1-1.075.015L2.22 6.53a.75.75 0 0 1 1.06-1.06l1.705 1.704l3.72-3.939a.75.75 0 0 1 1.06-.03Z"/></svg><span>20% affiliate marketing</span></li>
	</ul>
</div>

<Tokenomics />

<Roadmap>
	<RoadmapItem
		side=left
		quarter="Q2 2023"
		points={[
			'Integratly AI launch'
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
			'Develop a custom chat bot trading suite'
		]}
		done={[]}
	/>
</Roadmap>

<Testimonials />

<section id="footer" class="pt-16 pb-10">
	<div class="container">
		<div class="flex mb-6 gap-6 justify-center">
			<p class="text-body-color flex items-center"><a target="_blank" href="mailto:0xaigentx@gmail.com"><Icon icon=material-symbols:alternate-email-rounded style="font-size:32px" /></a></p>
			<p class="text-body-color flex items-center"><a target="_blank" href="https://twitter.com/0xAIgentx"><Icon icon=line-md:twitter-x-alt style="font-size:32px" /></a></p>
 			<p class="text-body-color flex items-center"><a target="_blank" href="https://t.me/+hWMgnOdPhG40Nzhl"><Icon icon=ph:telegram-logo-duotone style="font-size:32px" /></a></p>
			<p class="text-body-color flex items-center"><a target="_blank" href="https://aigentx.gitbook.io/whitepaper/"><Icon icon=material-symbols:lab-profile-rounded style="font-size:32px" /></a></p>
			

			<!-- <p class="text-body-color flex items-center"><a href="https://medium.com"><Icon icon=mdi:medium style="font-size:32px" /></a></p> -->
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