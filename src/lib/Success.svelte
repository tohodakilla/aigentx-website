<script>
	import airdrop from '$lib/images/airdrop.jpg'
	import bali from '$lib/images/baliagency.jpg'
	import tiger from '$lib/images/bnbtiger.jpg'
	import narfex from '$lib/images/narfex.jpg'

	export let items = [{}]

	const map = { airdrop, bali, tiger, narfex }
</script>

<section id="success" class="relative z-10 py-24">
	<div class="container">
			<div class="wow fadeInUp mx-auto mb-16 max-w-xxl text-center md:mb-20" data-wow-delay="0s">
				<span class="mb-3 text-lg font-bold uppercase text-primary sm:text-xl">Proven Success</span>
				<h2 class="mb-3 text-3xl font-bold leading-tight text-white md:text-[45px]">Integratly AI's Impactful Projects</h2>
				<p class="mx-auto max-w-[590px] text-lg font-medium text-body-color">At AIgentX, we thrive on real-world achievements, and our partnership with Integratly AI is a shining example. Join us as we explore some of our most impactful projects, demonstrating how Integratly AI's technology has already made a significant difference.</p>
			</div>

			<div class="-mx-4 flex flex-wrap justify-center">
				<div class="w-full px-4 lg:w-9/12 xl:w-8/12">
					{#each items as { head, text, link, button, img }}
						<a href="{link}" class="relative block single-faq wow fadeInUp mb-10 rounded-lg py-6 px-7 bg-dark md:py-8 md:px-10" data-wow-delay="0s">
							<div class="w-4/5">
								<h3 class="mr-2 text-base font-bold text-white sm:text-lg md:text-xl">{head}</h3>
	
								<div class="faq-content">
									<p class="text-relaxed pt-6 pb-9 text-base text-body-color">{text}</p>
								</div>
	
								<button class="rounded-lg bg-primary py-3 px-9 text-lg font-semibold text-white hover:bg-opacity-90 active:scale-95">{button}</button>
							</div>

							<img src={map[img]} alt="{button}" class="aspect-square object-cover absolute top-0 right-0 bottom-0 opacity-[0.69] w-1/5">
						</a>
					{/each}
				</div>
			</div>

			<div class="wow fadeInUp mx-auto mb-16 max-w-xxl text-center md:mb-20">
				<p class="mx-auto max-w-[590px] text-lg font-medium text-body-color">At AIgentX, we thrive on real-world achievements, and our partnership with Integratly AI is a shining example. Join us as we explore some of our most impactful projects, demonstrating how Integratly AI's technology has already made a significant difference.</p>
			</div>
		</div>

		<div class="absolute left-0 -bottom-36 -z-10">
			<img src="images/shapes/faq-shape-1.svg" alt="shape" />
		</div>
		<div class="absolute right-0 -top-36 -z-10">
			<img src="images/shapes/faq-shape-2.svg" alt="shape" />
		</div>
</section>