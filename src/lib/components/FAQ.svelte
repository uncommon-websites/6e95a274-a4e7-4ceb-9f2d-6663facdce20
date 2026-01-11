<script lang="ts">
	import { slide } from 'svelte/transition';

	const faqs = [
		{
			question: "How does Genaura pricing work?",
			answer: "Genaura charges based on the number of AWS resources under management. Contact us for custom enterprise pricing based on your infrastructure size."
		},
		{
			question: "How secure is connecting my AWS account?",
			answer: "Genaura uses AWS IAM roles with no credentials stored. You maintain full control over permissions and can revoke access anytime. All connections are encrypted and SOC 2 Type II compliant."
		},
		{
			question: "Does Genaura support multi-account AWS setups?",
			answer: "Yes, Genaura fully supports AWS Organizations and multi-account setups. You can manage all your AWS accounts from a single unified dashboard."
		},
		{
			question: "What AWS services does Genaura support?",
			answer: "Genaura supports all major AWS services including EC2, RDS, S3, Lambda, ECS, EKS, CloudFront, Route53, and more. We're constantly adding support for new services."
		},
		{
			question: "How does AutoHeal work?",
			answer: "AutoHeal uses AI to monitor your infrastructure 24/7, detect anomalies, and automatically fix common issues like unhealthy instances, connection pool exhaustion, and resource constraints."
		},
		{
			question: "Can I try Genaura before committing?",
			answer: "Yes, we offer a free trial with full access to all features. No credit card required. Import your AWS account in 60 seconds and see the value immediately."
		},
		{
			question: "What kind of cost savings can I expect?",
			answer: "Most customers see 30-40% reduction in AWS costs through AI-driven optimization, right-sizing recommendations, and automated cleanup of unused resources."
		}
	];

	let openIndex: number | null = null;

	function toggle(index: number) {
		openIndex = openIndex === index ? null : index;
	}
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto border-t border-gray-200">
	<div class="grid grid-cols-1 lg:grid-cols-3 gap-12">
		<div>
			<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
				[ FAQ ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl font-medium tracking-tight text-gray-900 mb-6">
				Frequently Asked Questions
			</h2>
			<p class="font-mono text-sm text-gray-600 mb-8">
				Your question not answered here?
			</p>
			<button class="bg-primary-600 text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-primary-700 transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs">
				<svg xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/></svg>
				Contact Us
			</button>
		</div>

		<div class="lg:col-span-2 space-y-4">
			{#each faqs as faq, i}
				<div class="border-b border-gray-200 pb-4">
					<button class="w-full flex items-center justify-between text-left py-2 group" on:click={() => toggle(i)}>
						<span class="text-sm font-medium text-gray-800 group-hover:text-primary-600 transition-colors pr-8">{faq.question}</span>
						<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-gray-400 transition-transform duration-300 {openIndex === i ? 'rotate-180' : ''}"><path d="m6 9 6 6 6-6"/></svg>
					</button>
					{#if openIndex === i}
						<div transition:slide={{ duration: 300 }} class="overflow-hidden">
							<p class="pt-2 pb-4 text-sm text-gray-600 leading-relaxed max-w-2xl">
								{faq.answer}
							</p>
						</div>
					{/if}
				</div>
			{/each}
		</div>
	</div>
</section>
