<script lang="ts">
	import { ShieldCheck, Bot, Scale, Globe } from 'lucide-svelte';
</script>

<section class="py-32 border-b border-white/5">
	<div class="max-w-[1400px] mx-auto px-6">
		<div class="text-center mb-24">
			<h2 class="text-4xl md:text-5xl font-serif">Built for Patent Prosecution Excellence</h2>
		</div>

		<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-x-8 gap-y-16">
			<div class="flex flex-col gap-6">
				<ShieldCheck size={28} class="text-white" strokeWidth={1.5} />
				<div>
					<h3 class="text-lg font-medium mb-3">Bank-Level Security</h3>
					<p class="text-gray-400 leading-relaxed text-sm">
						Your patent applications and client data are protected with enterprise-grade encryption and zero data training.
					</p>
				</div>
			</div>

			<div class="flex flex-col gap-6">
				<Bot size={28} class="text-white" strokeWidth={1.5} />
				<div>
					<h3 class="text-lg font-medium mb-3">Patent-Specific AI</h3>
					<p class="text-gray-400 leading-relaxed text-sm">
						AI models trained specifically on patent prosecution, understanding USPTO procedures and patent law nuances.
					</p>
				</div>
			</div>

			<div class="flex flex-col gap-6">
				<Scale size={28} class="text-white" strokeWidth={1.5} />
				<div>
					<h3 class="text-lg font-medium mb-3">30+ Years of Expertise</h3>
					<p class="text-gray-400 leading-relaxed text-sm">
						Founded by a patent prosecution attorney with decades of experience responding to Office Actions.
					</p>
				</div>
			</div>

			<div class="flex flex-col gap-6">
				<Globe size={28} class="text-white" strokeWidth={1.5} />
				<div>
					<h3 class="text-lg font-medium mb-3">Expert Support Team</h3>
					<p class="text-gray-400 leading-relaxed text-sm">
						Get help from patent professionals who understand your workflow and challenges.
					</p>
				</div>
			</div>
		</div>
	</div>
</section>
