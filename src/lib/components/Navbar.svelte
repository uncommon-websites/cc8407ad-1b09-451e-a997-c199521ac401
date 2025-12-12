<script lang="ts">
	import { ChevronDown, ArrowRight } from 'lucide-svelte';
</script>

<div class="fixed top-0 left-0 w-full z-50 bg-background/80 backdrop-blur-md border-b border-white/5">
	<!-- Top Banner -->
	<div class="bg-background text-[11px] text-gray-400 py-2.5 text-center border-b border-white/5 tracking-wide">
		Save 3+ hours on every Office Action response. <a href="#" class="text-white hover:text-gray-300 transition-colors inline-flex items-center gap-1 group">Learn how <ArrowRight size={10} class="group-hover:translate-x-0.5 transition-transform" /></a>
	</div>

	<!-- Navbar -->
	<nav class="max-w-[1400px] mx-auto px-6 h-16 flex items-center justify-between">
		<!-- Logo -->
		<a href="/" class="text-2xl font-sans tracking-tight text-white font-semibold">PatentReply<span class="text-primary-400">.ai</span></a>

		<!-- Links -->
		<div class="hidden md:flex items-center gap-8 text-[13px] font-medium text-gray-300">
			<button class="hover:text-white transition-colors flex items-center gap-1">
				Features <ChevronDown size={14} class="opacity-50" />
			</button>
			<a href="#" class="hover:text-white transition-colors">Pricing</a>
			<a href="#" class="hover:text-white transition-colors">Case Studies</a>
			<button class="hover:text-white transition-colors flex items-center gap-1">
				Resources <ChevronDown size={14} class="opacity-50" />
			</button>
			<a href="#" class="hover:text-white transition-colors">About</a>
		</div>

		<!-- Login -->
		<a href="#" class="text-[13px] font-medium text-white hover:text-gray-300 transition-colors">
			Login
		</a>
	</nav>
</div>
