<script lang="ts">
	// Logos - DevOps and Cloud companies
	const logos = [
		{ name: 'Vercel', width: 80 },
		{ name: 'Stripe', width: 90 },
		{ name: 'Notion', width: 80 },
		{ name: 'Linear', width: 70 },
		{ name: 'Supabase', width: 90 },
		{ name: 'Fly.io', width: 70 },
		{ name: 'Railway', width: 80 },
		{ name: 'Render', width: 80 },
		{ name: 'Planetscale', width: 100 },
		{ name: 'Neon', width: 60 }
	];
</script>

<section class="relative pt-32 pb-16 px-6 md:px-12 max-w-7xl mx-auto min-h-screen flex flex-col justify-between">
	<div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
		<div class="z-10">
			<h1 class="text-6xl md:text-7xl lg:text-8xl font-display font-medium text-gray-900 leading-[0.9] tracking-tight mb-8">
				Your AWS Console,<br><span class="text-primary-600">Self-Healing</span>
			</h1>
			
			<div class="space-y-6 max-w-lg">
				<p class="text-lg text-gray-600 leading-relaxed">
					Unified AWS management dashboard powered by AI. Connect via secure IAM roles, let AutoHeal fix issues automatically, and scale your cloud operations without the headcount.
				</p>

				<div class="flex flex-col items-start gap-3">
					<button class="bg-primary-600 text-white px-6 py-3 rounded text-sm font-medium hover:bg-primary-700 transition-colors flex items-center gap-2 shadow-sm">
						Start 60-Second Import
						<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14"/><path d="m12 5 7 7-7 7"/></svg>
					</button>
					<p class="text-[10px] text-gray-500 font-mono uppercase tracking-wide">
						Connect your AWS account in 60 seconds • No credit card required
					</p>
				</div>
			</div>
		</div>

		<div class="relative h-[400px] lg:h-[600px] w-full flex items-center justify-center">
			<!-- AWS Dashboard Visualization -->
			<div class="absolute inset-0 flex items-center justify-center">
				<div class="w-full max-w-lg bg-white rounded-lg shadow-2xl border border-gray-200 overflow-hidden">
					<!-- Mock Dashboard Header -->
					<div class="bg-gray-50 border-b border-gray-200 px-4 py-3 flex items-center justify-between">
						<div class="flex items-center gap-2">
							<div class="w-3 h-3 rounded-full bg-red-400"></div>
							<div class="w-3 h-3 rounded-full bg-yellow-400"></div>
							<div class="w-3 h-3 rounded-full bg-green-400"></div>
						</div>
						<span class="text-xs text-gray-500 font-mono">genaura.cloud</span>
					</div>
					<!-- Mock Dashboard Content -->
					<div class="p-6 space-y-4">
						<div class="flex items-center justify-between">
							<div class="text-sm font-medium text-gray-900">AWS Resources</div>
							<div class="text-xs text-primary-600 font-mono">● Live</div>
						</div>
						<div class="grid grid-cols-3 gap-3">
							<div class="bg-gray-50 rounded p-3 border border-gray-200">
								<div class="text-xs text-gray-500 mb-1">EC2</div>
								<div class="text-lg font-bold text-gray-900">24</div>
							</div>
							<div class="bg-gray-50 rounded p-3 border border-gray-200">
								<div class="text-xs text-gray-500 mb-1">RDS</div>
								<div class="text-lg font-bold text-gray-900">8</div>
							</div>
							<div class="bg-gray-50 rounded p-3 border border-gray-200">
								<div class="text-xs text-gray-500 mb-1">S3</div>
								<div class="text-lg font-bold text-gray-900">156</div>
							</div>
						</div>
						<div class="bg-primary-50 border border-primary-200 rounded p-3 flex items-start gap-2">
							<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-primary-600 shrink-0 mt-0.5"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg>
							<div class="text-xs text-primary-900">
								<span class="font-bold">AutoHeal:</span> Fixed 3 issues in the last hour
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>

	<div class="mt-20 border-t border-gray-300 pt-8">
		<div class="flex items-center gap-2 text-[10px] font-mono uppercase tracking-wider text-gray-600 mb-6">
			Trusted by DevOps teams running AWS at scale
		</div>
		
		<div class="grid grid-cols-2 md:grid-cols-5 gap-8 opacity-60 grayscale">
			{#each logos as logo}
				<div class="h-8 flex items-center justify-center border border-gray-300/50 rounded bg-gray-100/50">
					<span class="text-xs font-bold text-gray-500">{logo.name}</span>
				</div>
			{/each}
		</div>
	</div>
</section>
