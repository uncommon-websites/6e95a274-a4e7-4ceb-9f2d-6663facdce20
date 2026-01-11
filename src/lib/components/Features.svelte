<script lang="ts">
	import FeatureCard from './FeatureCard.svelte';
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto relative" id="features">
    <!-- Background Grid Pattern -->
    <div class="absolute inset-0 z-0 opacity-30 pointer-events-none" 
        style="background-image: linear-gradient(#ccc 1px, transparent 1px), linear-gradient(90deg, #ccc 1px, transparent 1px); background-size: 40px 40px; mask-image: linear-gradient(to bottom, transparent, black 10%, black 90%, transparent);">
    </div>

	<div class="flex flex-col md:flex-row justify-between items-start md:items-end mb-16 gap-6 relative z-10">
		<div>
			<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
				[ POWERFUL FEATURES ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-4">
				Everything you need to<br>manage AWS at scale.
			</h2>
			<p class="text-sm text-gray-600 max-w-lg">
				Replace your AWS console with a unified, AI-powered dashboard that connects securely and scales with your team.
			</p>
		</div>
		
		<button class="bg-black text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-gray-800 transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs">
			View Demo ->
		</button>
	</div>

	<div class="grid grid-cols-1 md:grid-cols-2 gap-6">
		<FeatureCard 
			subtitle="[ UNIFIED DASHBOARD ]"
			title="All your AWS resources<br>in one place"
			description="View and manage EC2, RDS, S3, Lambda, and all AWS services from a single, intuitive interface."
			tagColor="bg-primary-600"
			tagIcon="arrow"
            imageSrc="https://placehold.co/600x400/FFFFFF/E5E7EB?text=Unified+Dashboard"
		/>
		
		<FeatureCard 
			subtitle="[ AUTOHEAL ]"
			title="Self-healing infrastructure<br>powered by AI"
			description="AI automatically detects and fixes common AWS issues before they impact your users. Reduce on-call burden."
			tagColor="bg-accent-orange"
			tagIcon="plus"
            imageSrc="https://placehold.co/600x400/FFFFFF/E5E7EB?text=AutoHeal+AI"
		/>
		
		<FeatureCard 
			subtitle="[ SECURE IAM ]"
			title="Connect via secure<br>IAM roles"
			description="No credentials stored. Connect your AWS account through secure IAM roles with granular permissions."
			tagColor="bg-accent-pink"
			tagIcon="arrow"
            imageSrc="https://placehold.co/600x400/FFFFFF/E5E7EB?text=IAM+Security"
		/>
		
		<FeatureCard 
			subtitle="[ COST OPTIMIZATION ]"
			title="Save on AWS costs<br>automatically"
			description="AI-driven insights identify wasteful spending and optimize resource allocation to reduce your AWS bill."
			tagColor="bg-accent-yellow"
			tagIcon="plus"
            imageSrc="https://placehold.co/600x400/FFFFFF/E5E7EB?text=Cost+Savings"
		/>
	</div>
</section>
