<section class="bg-primary-50 py-24 px-6 md:px-12 relative overflow-hidden">
	<div class="max-w-7xl mx-auto grid grid-cols-1 lg:grid-cols-2 gap-12 items-center relative z-10">
		<div>
			<span class="font-mono text-[10px] text-primary-700 uppercase tracking-widest mb-4 block">
				[ COMPLETE VISIBILITY ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-6 leading-[0.95]">
				Visualize Your<br>AWS Infrastructure
			</h2>
			<p class="text-sm text-gray-700 max-w-md mb-8 leading-relaxed">
				Genaura maps your entire AWS infrastructure and understands dependencies between services. See how everything connects in real-time.
			</p>
			
			<button class="bg-primary-600 text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-primary-700 transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs w-fit">
				Explore Infrastructure View ->
			</button>
		</div>

		<div class="relative h-[400px] w-full flex items-center justify-center">
			<!-- AWS Infrastructure Graph -->
			<div class="absolute inset-0">
				<svg width="100%" height="100%" viewBox="0 0 400 300" class="overflow-visible">
					<!-- Edges -->
                    <g stroke="oklch(0.685 0.169 237.323)" stroke-width="1" opacity="0.3">
                        <line x1="200" y1="150" x2="150" y2="100" />
                        <line x1="200" y1="150" x2="250" y2="100" />
                        <line x1="200" y1="150" x2="150" y2="200" />
                        <line x1="200" y1="150" x2="250" y2="200" />
                        <line x1="150" y1="100" x2="100" y2="150" />
                        <line x1="250" y1="100" x2="300" y2="150" />
                        <line x1="150" y1="200" x2="100" y2="150" />
                        <line x1="250" y1="200" x2="300" y2="150" />
                        <line x1="150" y1="100" x2="180" y2="80" />
                        <line x1="250" y1="100" x2="220" y2="80" />
                    </g>
					<!-- Nodes with AWS service labels -->
                    <g>
                        <!-- Central node - VPC -->
                        <circle cx="200" cy="150" r="8" fill="oklch(0.685 0.169 237.323)" stroke="#fff" stroke-width="2" />
                        <text x="200" y="175" text-anchor="middle" font-size="10" fill="#374151" font-weight="bold">VPC</text>
                        
                        <!-- EC2 -->
                        <circle cx="150" cy="100" r="6" fill="oklch(0.685 0.169 237.323)" stroke="#fff" stroke-width="2" />
                        <text x="150" y="90" text-anchor="middle" font-size="9" fill="#374151">EC2</text>
                        
                        <!-- RDS -->
                        <circle cx="250" cy="100" r="6" fill="oklch(0.685 0.169 237.323)" stroke="#fff" stroke-width="2" />
                        <text x="250" y="90" text-anchor="middle" font-size="9" fill="#374151">RDS</text>
                        
                        <!-- Lambda -->
                        <circle cx="150" cy="200" r="6" fill="oklch(0.685 0.169 237.323)" stroke="#fff" stroke-width="2" />
                        <text x="150" y="215" text-anchor="middle" font-size="9" fill="#374151">Lambda</text>
                        
                        <!-- S3 -->
                        <circle cx="250" cy="200" r="6" fill="oklch(0.685 0.169 237.323)" stroke="#fff" stroke-width="2" />
                        <text x="250" y="215" text-anchor="middle" font-size="9" fill="#374151">S3</text>
                        
                        <!-- ALB -->
                        <circle cx="100" cy="150" r="5" fill="oklch(0.685 0.169 237.323)" stroke="#fff" stroke-width="2" />
                        <text x="100" y="140" text-anchor="middle" font-size="8" fill="#374151">ALB</text>
                        
                        <!-- CloudFront -->
                        <circle cx="300" cy="150" r="5" fill="oklch(0.685 0.169 237.323)" stroke="#fff" stroke-width="2" />
                        <text x="300" y="140" text-anchor="middle" font-size="8" fill="#374151">CF</text>
                        
                        <!-- Additional services -->
                        <circle cx="180" cy="80" r="4" fill="oklch(0.685 0.169 237.323)" stroke="#fff" stroke-width="1" />
                        <circle cx="220" cy="80" r="4" fill="oklch(0.685 0.169 237.323)" stroke="#fff" stroke-width="1" />
                    </g>
				</svg>
			</div>
		</div>
	</div>
    
    <!-- Background Grid Pattern -->
    <div class="absolute inset-0 z-0 opacity-10" 
        style="background-image: linear-gradient(#000 1px, transparent 1px), linear-gradient(90deg, #000 1px, transparent 1px); background-size: 40px 40px;">
    </div>
</section>
