<script>
	import { reveal } from 'svelte-reveal'
</script>

<section id="try" class="pt-[120px] pb-20">
	<div class="container">
		<div class="wow fadeInUp mx-auto mb-16 max-w-[590px] text-center md:mb-20" use:reveal={{ delay: 0 }}>
			<!-- <span class="mb-3 text-lg font-bold uppercase text-primary sm:text-xl">No Hype, Just Results!</span> -->
			<h2 class="mb-3 text-3xl font-bold leading-tight text-white md:text-[45px]">Try It Now - No Empty Promises</h2>
			<!--<p class="text-lg font-medium text-body-color-2 dark:text-body-color"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc sed congue arcu, In et dignissim quam condimentum vel. </p> -->
		</div>
		
		<div class="-mx-4 grid grid-cols-1 lg:grid-cols-2 grid-rows-2 lg:grid-rows-1 gap-6">
				<div class="group rounded-lg border-b-4 border-transparent p-4 text-center transition-all hover:border-primary bg-dark" use:reveal={{ delay: 0 }}>

					<h3 class="mb-6 text-2xl font-semibold text-body-color">AI Bot: Powered by Real Innovation, Not Hype</h3>
					<p class="mb-3 text-base font-medium text-body-color">We don't just talk about groundbreaking technology; we've actually built it. Experience our AI chatbot for yourself by interacting with it live. We believe in showing, not telling.</p>
					<p class="mb-3 text-base font-medium text-body-color">Access our bot through the:</p>
					<div class="mb-4 flex items-center justify-center space-x-4">
						<button 
						on:click={() => document?.querySelector('.amo-button--main-icon').click()}
						class="rounded-lg bg-primary py-3 px-6 text-lg font-semibold text-white hover:bg-opacity-90 active:scale-95">Live Chat</button>
						<a href="https://t.me/AIgentX_aibot" class="rounded-lg bg-primary py-3 px-6 text-lg font-semibold text-white hover:bg-opacity-90 active:scale-95">Telegram Bot</a>
					</div>
				</div>

				<div class="group rounded-lg border-b-4 border-transparent p-4 text-center transition-all hover:border-primary bg-dark" use:reveal={{ delay: 0 }}>
					<h3 class="mb-6 text-2xl font-semibold text-body-color">AIX Token Holders: Get Ready for More Power</h3>
					<p class="mb-3 text-base font-medium text-body-color">Are you an AIX token holder? Get ready for exclusive benefits. We're in the final stages of launching an AI chatbot builder that will allow you to set up your very own AI bot—for free. While we're fine-tuning this amazing feature, you can express your interest by sending us an email request. Don't miss out on turning your AIX tokens into real utility.</p>
					<h4 class="mb-2 text-lg font-semibold text-body-color">AI Bot Builder Coming Soon</h4>
				</div>
		</div>
	</div>
</section>