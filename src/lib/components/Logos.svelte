<script lang="ts">
	import { ChevronRight } from 'lucide-svelte';
</script>

<section class="py-12 border-b border-white/5">
	<div class="max-w-[1400px] mx-auto px-6">
		<div class="text-center mb-10">
			<p class="text-xl font-serif text-gray-200">Trusted by Patent Professionals</p>
		</div>

		<!-- Logos Grid - Using text for now as I don't have the SVGs, but styling to look like logos -->
		<div class="flex flex-wrap justify-center items-center gap-x-16 gap-y-10 opacity-60 grayscale hover:grayscale-0 transition-all duration-500">
			<span class="text-lg font-serif font-bold tracking-widest text-white">FISH & RICHARDSON</span>
			<span class="text-xl font-serif font-bold tracking-widest text-white">FINNEGAN</span>
			<span class="text-xl font-sans font-bold text-white">KILPATRICK</span>
			<span class="text-lg font-sans font-bold text-white">STERNE KESSLER</span>
			<span class="text-2xl font-serif text-white">Cooley</span>
			<span class="text-xl font-sans font-black tracking-tighter text-white">WilmerHale</span>
			<span class="text-xl font-serif text-white">Morrison Foerster</span>
		</div>

		<div class="text-center mt-12">
			<a href="#" class="text-sm text-gray-400 hover:text-white transition-colors inline-flex items-center gap-1">
				See Case Studies <ChevronRight size={12} />
			</a>
		</div>
	</div>
</section>
