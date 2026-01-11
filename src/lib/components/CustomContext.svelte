<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto">
	<div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-center">
		<div>
			<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
				[ 60-SECOND SETUP ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-6 leading-[0.95]">
				Import your AWS<br>in 60 seconds.
			</h2>
			<p class="text-sm text-gray-600 max-w-md mb-12">
				Connect your AWS account securely and start managing your infrastructure immediately. No complex migration required.
			</p>

			<div class="space-y-12 relative">
                <!-- Vertical line connecting steps -->
                <div class="absolute left-[11px] top-2 bottom-2 w-[1px] bg-gray-200 -z-10"></div>

				<div class="flex gap-6 group">
					<div class="w-6 h-6 rounded-full bg-primary-600 border border-primary-600 flex items-center justify-center text-xs font-mono text-white shrink-0 shadow-sm">1</div>
					<div>
						<h3 class="font-bold text-gray-900 mb-2">Create secure IAM role</h3>
						<p class="text-sm text-gray-600 leading-relaxed max-w-sm">
							Follow our one-click CloudFormation template to create a secure IAM role with read-only or admin permissions.
						</p>
					</div>
				</div>

				<div class="flex gap-6 group">
					<div class="w-6 h-6 rounded-full bg-gray-100 border border-gray-300 flex items-center justify-center text-xs font-mono text-gray-500 shrink-0 group-hover:bg-primary-600 group-hover:border-primary-600 group-hover:text-white transition-colors">2</div>
					<div>
						<h3 class="font-bold text-gray-900 mb-2">Connect your AWS account</h3>
						<p class="text-sm text-gray-600 leading-relaxed max-w-sm">
							Enter your AWS account ID and role ARN. Genaura automatically imports your infrastructure.
						</p>
					</div>
				</div>

				<div class="flex gap-6 group">
					<div class="w-6 h-6 rounded-full bg-gray-100 border border-gray-300 flex items-center justify-center text-xs font-mono text-gray-500 shrink-0 group-hover:bg-primary-600 group-hover:border-primary-600 group-hover:text-white transition-colors">3</div>
					<div>
						<h3 class="font-bold text-gray-900 mb-2">Start managing your infrastructure</h3>
						<p class="text-sm text-gray-600 leading-relaxed max-w-sm">
							View all resources, enable AutoHeal, and replace your AWS console with Genaura's unified dashboard.
						</p>
					</div>
				</div>
			</div>
			
			<div class="mt-12">
				<button class="bg-black text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-gray-800 transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs">
					View Setup Guide ->
				</button>
			</div>
		</div>

		<div class="bg-[#F3F3F1] p-2 rounded-lg border border-gray-200 shadow-sm">
            <div class="bg-white rounded border border-gray-200 overflow-hidden p-6">
				<!-- Mock IAM Setup UI -->
				<div class="space-y-4">
					<div class="flex items-center justify-between pb-3 border-b border-gray-200">
						<h3 class="font-bold text-gray-900">Connect AWS Account</h3>
						<span class="text-xs bg-primary-100 text-primary-700 px-2 py-1 rounded font-mono">Step 2 of 3</span>
					</div>
					<div>
						<label class="block text-xs font-medium text-gray-700 mb-2">AWS Account ID</label>
						<input type="text" value="123456789012" class="w-full border border-gray-300 rounded px-3 py-2 text-sm font-mono bg-gray-50" readonly />
					</div>
					<div>
						<label class="block text-xs font-medium text-gray-700 mb-2">IAM Role ARN</label>
						<input type="text" value="arn:aws:iam::123456789012:role/GenauraAccess" class="w-full border border-gray-300 rounded px-3 py-2 text-sm font-mono bg-gray-50" readonly />
					</div>
					<div class="bg-green-50 border border-green-200 rounded p-3 flex items-start gap-2">
						<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-green-600 shrink-0 mt-0.5"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"/><polyline points="22 4 12 14.01 9 11.01"/></svg>
						<span class="text-xs text-green-800">IAM role verified successfully</span>
					</div>
					<button class="w-full bg-primary-600 text-white py-2.5 rounded text-sm font-medium hover:bg-primary-700 transition-colors">
						Import AWS Resources
					</button>
				</div>
            </div>
		</div>
	</div>
</section>
