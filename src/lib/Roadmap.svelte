<section id="roadmap" class="relative z-10 py-[120px]">
	<div class="container">
		<div class="wow fadeInUp mx-auto mb-16 max-w-[590px] text-center md:mb-20" data-wow-delay="0s">
			<!-- <span class="mb-3 text-lg font-bold uppercase text-primary sm:text-xl"> ROADMAP </span> -->
			<h2 class="mb-3 text-3xl font-bold leading-tight text-white md:text-[45px]"> ROADMAP </h2>
			<p class="text-lg font-medium text-body-color"><strong>Testnet Launch:</strong> September 8th 2023</p>
		</div>

		<div class="-mx-4 flex justify-center">
			<div class="w-full px-4 lg:w-10/12 xl:w-9/12">
				<div class="wow fadeInUp relative -mx-4 flex flex-wrap md:py-14 lg:py-20" data-wow-delay="0s">
					<span class="absolute top-0 left-2 hidden h-full w-[2px] bg-[#2D2C4A] md:left-1/2 md:block"></span>
					
					<slot />
					
				</div>

				<div class="absolute left-0 bottom-0 -z-10">
					<img src="images/shapes/timeline.svg" alt="shape" />
				</div>
			</div>
		</div>
	</div>


</section>