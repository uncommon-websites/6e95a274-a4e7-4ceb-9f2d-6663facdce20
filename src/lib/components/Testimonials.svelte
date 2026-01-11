<script lang="ts">
	const testimonials = [
		{
			quote: "Genaura replaced our AWS console and cut our cloud ops time in half. The AutoHeal feature alone has saved us countless hours of on-call firefighting.",
			author: "Sarah Chen",
			role: "VP Engineering • Stripe",
			image: "https://i.pravatar.cc/150?u=sarah",
            icon: "https://placehold.co/20x20/635BFF/fff?text=S"
		},
		{
			quote: "We were drowning in AWS console complexity. Genaura's unified dashboard gave us visibility we never had before, and the 60-second import was no joke.",
			author: "Marcus Johnson",
			role: "DevOps Lead • Vercel",
			image: "https://i.pravatar.cc/150?u=marcus",
            icon: "https://placehold.co/20x20/000/fff?text=V"
		},
		{
			quote: "The cost savings alone paid for Genaura in the first month. AI-driven optimization found waste we didn't even know existed.",
			author: "Priya Patel",
			role: "CTO • Notion",
			image: "https://i.pravatar.cc/150?u=priya",
            icon: "https://placehold.co/20x20/000/fff?text=N"
		},
		{
			quote: "AutoHeal is like having a senior DevOps engineer working 24/7. It catches and fixes issues before they become incidents.",
			author: "Alex Rivera",
			role: "Infrastructure Lead • Linear",
			image: "https://i.pravatar.cc/150?u=alex",
            icon: "https://placehold.co/20x20/5E6AD2/fff?text=L"
		},
		{
			quote: "Security was our biggest concern, but the IAM role approach is brilliant. No credentials stored, full audit trail, and we maintain complete control.",
			author: "Jordan Kim",
			role: "Security Engineer • Supabase",
			image: "https://i.pravatar.cc/150?u=jordan",
            icon: "https://placehold.co/20x20/3ECF8E/fff?text=S"
		},
		{
			quote: "We scaled from 50 to 500 AWS resources without adding DevOps headcount. Genaura made that possible.",
			author: "Taylor Brooks",
			role: "CTO • Railway",
			image: "https://i.pravatar.cc/150?u=taylor",
            icon: "https://placehold.co/20x20/0B0D0E/fff?text=R"
		},
        {
			quote: "The infrastructure visualization alone is worth it. Finally understand how all our AWS services connect and depend on each other.",
			author: "Chris Anderson",
			role: "Platform Engineer • Render",
			image: "https://i.pravatar.cc/150?u=chris",
            icon: "https://placehold.co/20x20/46E3B7/fff?text=R"
		},
        {
			quote: "Setup took literally 60 seconds. Within an hour we had full visibility into our entire AWS infrastructure. Game changer for our team.",
			author: "Jamie Lee",
			role: "DevOps Manager • Fly.io",
			image: "https://i.pravatar.cc/150?u=jamie",
            icon: "https://placehold.co/20x20/7B3FF2/fff?text=F"
		}
	];
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto">
	<div class="text-center mb-16">
		<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
			[ TESTIMONIALS ]
		</span>
		<h2 class="font-display text-4xl md:text-5xl font-medium tracking-tight text-gray-900 mb-4">
			Trusted by DevOps Teams
		</h2>
		<p class="text-sm text-gray-600">
			See what engineering leaders are saying about Genaura
		</p>
	</div>

	<div class="columns-1 md:columns-2 lg:columns-3 gap-6 space-y-6">
		{#each testimonials as t}
			<div class="bg-white p-6 rounded-lg border border-gray-200 shadow-sm break-inside-avoid hover:shadow-md transition-shadow">
				<p class="font-mono text-xs leading-relaxed text-gray-700 mb-6">
					"{t.quote}"
				</p>
				<div class="flex items-center justify-between border-t border-gray-100 pt-4">
					<div class="flex items-center gap-3">
						<img src={t.image} alt={t.author} class="w-8 h-8 rounded-full bg-gray-200" />
						<div>
							<div class="text-xs font-bold text-gray-900">{t.author}</div>
							<div class="text-[10px] text-gray-500 font-mono">{t.role}</div>
						</div>
					</div>
                    <img src={t.icon} alt="Company Logo" class="w-5 h-5 rounded-sm opacity-70 grayscale" />
				</div>
			</div>
		{/each}
	</div>
</section>
