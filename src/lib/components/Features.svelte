<script lang="ts">
	import FeatureSection from './FeatureSection.svelte';
	import { FileText, Shield, Zap, Search, Globe, Scale } from 'lucide-svelte';
</script>

<section>
	<div class="py-24 text-center border-b border-white/5">
		<h2 class="text-3xl md:text-4xl font-serif">
			Everything You Need to Respond <br />
			to Office Actions Faster
		</h2>
	</div>

	<!-- Feature 1: Rejection Analysis -->
	<FeatureSection
		title="Rejection Analysis"
		subtitle="Understand Rejections Instantly"
		description="AI-powered analysis breaks down complex Office Action rejections, identifying key issues and suggesting response strategies."
		linkText="Learn More"
		reversed={false}
	>
		<!-- Rejection Analysis UI Mockup -->
		<div class="bg-white text-black p-8 rounded shadow-2xl w-full max-w-md relative">
			<p class="mb-6 font-serif text-lg leading-relaxed">
				The examiner has rejected claims 1-15 under 35 U.S.C. § 103 as obvious over Smith (US 2020/0123456) in view of Jones (US 9,876,543). <sup class="bg-gray-200 px-1 rounded text-xs">1</sup> The primary reference Smith discloses elements A, B, and C of claim 1. <sup class="bg-gray-200 px-1 rounded text-xs">2</sup> Jones teaches element D in the context of a similar technical field. <sup class="bg-gray-200 px-1 rounded text-xs">3</sup> Recommended strategy: Amend claim 1 to include feature E from dependent claim 5, which is not disclosed in either reference...
			</p>
			<div class="absolute bottom-4 right-4 w-3 h-3 bg-primary-400 rounded-full animate-pulse"></div>
		</div>
	</FeatureSection>

	<!-- Feature 2: Claim Amendment Testing -->
	<FeatureSection
		title="Amendment Testing"
		subtitle="Test Claims Before Filing"
		description="Validate proposed claim amendments against cited prior art and identify potential issues before you respond."
		linkText="Learn More"
		reversed={true}
	>
		<!-- Amendment Testing UI Mockup -->
		<div class="w-full max-w-sm">
			<div class="bg-white text-black p-8 rounded shadow-2xl aspect-[4/3] flex flex-col items-center justify-center gap-6">
				<div class="w-full">
					<div class="flex items-center justify-between mb-2">
						<span class="text-sm font-semibold">Claim Strength</span>
						<span class="text-2xl font-bold text-green-600">92%</span>
					</div>
					<div class="w-full bg-gray-200 rounded-full h-3">
						<div class="bg-green-500 h-3 rounded-full" style="width: 92%"></div>
					</div>
				</div>
				<div class="w-full text-xs space-y-2">
					<div class="flex items-center gap-2">
						<div class="w-2 h-2 bg-green-500 rounded-full"></div>
						<span>No overlap with Smith reference</span>
					</div>
					<div class="flex items-center gap-2">
						<div class="w-2 h-2 bg-green-500 rounded-full"></div>
						<span>Feature E not disclosed in Jones</span>
					</div>
					<div class="flex items-center gap-2">
						<div class="w-2 h-2 bg-yellow-500 rounded-full"></div>
						<span>Consider narrowing element B</span>
					</div>
				</div>
			</div>
		</div>
	</FeatureSection>

	<!-- Feature 3: Document Management -->
	<FeatureSection
		title="Document Hub"
		subtitle="All Your Files, Organized"
		description="Upload and analyze Office Actions, specifications, and prior art references in one secure workspace."
		linkText="Learn More"
		reversed={false}
	>
		<!-- Document Hub UI Mockup -->
		<div class="bg-white text-black p-6 rounded shadow-2xl w-full max-w-md text-xs">
			<div class="grid grid-cols-3 gap-4 mb-4 font-semibold border-b pb-2">
				<div>Document</div>
				<div>Type</div>
				<div>Status</div>
			</div>
			{#each [
				{ name: 'Office Action', type: 'OA', status: 'Analyzed' },
				{ name: 'Smith Patent', type: 'Prior Art', status: 'Reviewed' },
				{ name: 'Jones Patent', type: 'Prior Art', status: 'Reviewed' },
				{ name: 'Application', type: 'Spec', status: 'Active' },
				{ name: 'Amendment Draft', type: 'Response', status: 'In Progress' },
				{ name: 'IDS References', type: 'Prior Art', status: 'Pending' },
				{ name: 'Claims Chart', type: 'Analysis', status: 'Complete' }
			] as doc}
				<div class="grid grid-cols-3 gap-4 mb-3 opacity-60">
					<div class="h-2 bg-gray-200 rounded w-3/4"></div>
					<div class="h-2 bg-gray-200 rounded w-full"></div>
					<div class="h-2 bg-gray-200 rounded w-5/6"></div>
				</div>
			{/each}
		</div>
	</FeatureSection>

	<!-- Feature 4: Response Workflows -->
	<FeatureSection
		title="Smart Workflows"
		subtitle="Automated Response Prep"
		description="Pre-built workflows guide you through every step of Office Action response preparation, from analysis to final review."
		linkText="Learn More"
		reversed={true}
	>
		<!-- Workflows UI Mockup -->
		<div class="grid grid-cols-2 gap-4 w-full max-w-md">
			<div class="bg-white text-black p-6 rounded shadow-lg flex flex-col items-center text-center gap-4 aspect-square justify-center hover:scale-[1.02] transition-transform duration-300">
				<Search size={32} strokeWidth={1.5} />
				<span class="font-medium text-lg">Prior Art Search</span>
			</div>
			<div class="bg-white text-black p-6 rounded shadow-lg flex flex-col items-center text-center gap-4 aspect-square justify-center hover:scale-[1.02] transition-transform duration-300">
				<FileText size={32} strokeWidth={1.5} />
				<span class="font-medium text-lg">Claims Analysis</span>
			</div>
			<div class="bg-white text-black p-6 rounded shadow-lg flex flex-col items-center text-center gap-4 aspect-square justify-center hover:scale-[1.02] transition-transform duration-300">
				<Scale size={32} strokeWidth={1.5} />
				<span class="font-medium text-lg">Amendment Draft</span>
			</div>
			<div class="bg-white text-black p-6 rounded shadow-lg flex flex-col items-center text-center gap-4 aspect-square justify-center hover:scale-[1.02] transition-transform duration-300">
				<Zap size={32} strokeWidth={1.5} />
				<span class="font-medium text-lg">Response Review</span>
			</div>
		</div>
	</FeatureSection>
</section>
