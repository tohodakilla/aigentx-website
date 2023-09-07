<script>
	import kris from '$lib/images/kris.webp'
	import jusuf from '$lib/images/Jusuf.webp'
</script>

<section id="testimonial" class="pt-[120px] pb-20 bg-[#14102C]">
	<div class="container">
		<div class="wow fadeInUp mx-auto mb-16 max-w-[590px] text-center md:mb-20" data-wow-delay="0s">
			<span class="mb-3 text-lg font-bold uppercase text-primary sm:text-xl">TESTIMONIALS</span>
			<h2 class="mb-3 text-3xl font-bold leading-tight text-white md:text-[45px]">What Our Client Say's</h2>
			<!-- <p class="text-lg font-medium text-body-color-2 dark:text-body-color">
	  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc sed
	  congue arcu, In et dignissim quam condimentum vel.
	</p> -->
		</div>

		<div class="-mx-4 flex flex-wrap">
			<div class="w-full px-4 md:w-1/2">
				<div class="wow fadeInUp relative z-10 mb-10 overflow-hidden rounded-[10px] px-6 py-8 bg-[#131B4D] sm:p-10 md:p-8 xl:p-10" data-wow-delay="0s">
					<div class="absolute right-0 top-0 z-[-1]">
						<img src="images/shapes/testimonial-shape.svg" alt="shape" />
					</div>
					
					<h3 class="mb-1 text-lg font-bold text-white">A Real Game Changer for Our Sales</h3>
					<p class="mb-8 text-base font-medium leading-snug text-body-color-2 dark:text-body-color">“So, we've recently integrated SalesBot AI into our business operations at Welcome to Bali Visa agency. Honestly? I'm still surprised at how much SalesBot AI has transformed our sales process at Bali Visa. The bot managed to close 28 visas in its first week alone - absolutely amazing!”</p>
					<div class="flex items-start">
						<div class="mr-5 h-20 w-full max-w-[80px] overflow-hidden rounded">
							<img src={kris} alt="Kris" />
						</div>
						<div class="w-full">
						
							<h3 class="mb-1 text-md font-semibold text-white">Kris</h3>
							<p class="text-sm font-medium text-white mb-6">WelcomeToBali Visa Agency</p>
							<a class="font-bold underline" href="https://t.me/WelcomeToBali_bot">Link to bot</a>
						</div>
					</div>	
				</div>
			</div>

			<div class="w-full px-4 md:w-1/2">
				<div class="wow fadeInUp relative z-10 mb-10 overflow-hidden rounded-[10px] px-6 py-8 bg-[#131B4D] sm:p-10 md:p-8 xl:p-10" data-wow-delay="0s">
					<div class="absolute right-0 top-0 z-[-1]">
						<img src="images/shapes/testimonial-shape.svg" alt="shape" />
					</div>
					
					<h3 class="mb-1 text-lg font-bold text-white">The Best Investment We've Made</h3>
					<p class="mb-8 text-base font-medium leading-snug text-body-color-2 dark:text-body-color">“You know, I was a bit skeptical about the whole AI thing. But SalesBot AI has genuinely impressed me! Our support costs have dropped by an astonishing 32%, and the best part is - it never sleeps. Queries are handled accurately and instantly, keeping our customers satisfied round the clock.”</p>
					<div class="flex items-start">
						<div class="mr-5 h-20 w-full max-w-[80px] overflow-hidden rounded">
							<img src={jusuf} alt="Jusuf" />
						</div>
						
						<div class="w-full">
							<h3 class="mb-1 text-md font-semibold text-white">Yusuf Ghairat</h3>
							<p class="text-sm font-medium text-white mb-6">Narfex - Currency Exchange</p>
							<a class="font-bold underline" href="https://t.me/NarfexAI_bot">Link to bot</a>
						</div>
					</div>	
				</div>
			</div>
		</div>
	</div>
</section>