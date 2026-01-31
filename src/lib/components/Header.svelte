<script lang="ts">
	import { onMount } from 'svelte';
	
	let isScrolled = false;

	onMount(() => {
		const handleScroll = () => {
			isScrolled = window.scrollY > 20;
		};
		window.addEventListener('scroll', handleScroll);
		return () => window.removeEventListener('scroll', handleScroll);
	});
</script>

<header class="fixed top-0 left-0 right-0 z-50 transition-all duration-300 px-6 py-4 flex items-center justify-between {isScrolled ? 'bg-[#EAEAE8]/90 backdrop-blur-md border-b border-gray-200' : 'bg-transparent'}">
	<div class="flex items-center gap-8">
		<a href="/" class="flex items-center gap-2 text-brand-dark font-medium text-xl tracking-tight">
			<div class="w-6 h-6 text-primary-600">
				<svg viewBox="0 0 97 105" fill="none" xmlns="http://www.w3.org/2000/svg">
					<path opacity="0.5" d="M0.84375 29.5892V75.3785L43.791 45.7896V0L0.84375 29.5892Z" fill="currentColor"/>
					<path opacity="0.5" d="M0.84375 75.3787V29.5891L43.791 59.1783V104.968L0.84375 75.3787Z" fill="currentColor"/>
					<path opacity="0.5" d="M96.8438 29.5891V75.3787L53.8965 45.7895V0L96.8438 29.5891Z" fill="currentColor"/>
					<path opacity="0.5" d="M96.8438 75.3787V29.5891L53.8965 59.1783V104.968L96.8438 75.3787Z" fill="currentColor"/>
				</svg>
			</div>
			Genaura
		</a>
		
		<nav class="hidden md:flex items-center gap-6 text-sm font-medium text-gray-600">
			<a href="#features" class="hover:text-gray-900 transition-colors">Features</a>
			<a href="#pricing" class="hover:text-gray-900 transition-colors">Pricing</a>
			<a href="#security" class="hover:text-gray-900 transition-colors">Security</a>
			<button class="flex items-center gap-1 hover:text-gray-900 transition-colors group">
				Resources
				<svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="group-hover:rotate-180 transition-transform"><path d="m6 9 6 6 6-6"/></svg>
			</button>
			<a href="#docs" class="hover:text-gray-900 transition-colors">Docs</a>
		</nav>
	</div>

	<div class="flex items-center gap-4">
		<a href="#signin" class="text-sm font-medium text-gray-700 hover:text-gray-900 transition-colors">Sign In</a>
		<a href="#start" class="text-sm font-medium text-white bg-primary-600 px-4 py-2 rounded hover:bg-primary-700 transition-colors shadow-sm">Get Started</a>
	</div>
</header>
