<script>
	import '../app.css';
	import Navbar from '$lib/components/layout/navbar.svelte';
	import About from './sections/about.svelte';
	import Origin from './sections/origin.svelte';
	import Features from './sections/features.svelte';
	import Team from './sections/team.svelte';
	import Testimonial from './sections/testimonial.svelte';
	import Faqs from './sections/faqs.svelte';
	import Footer from '$lib/components/layout/footer.svelte';
	let { children } = $props();
</script>

<div class="relative min-h-screen w-full m-0 p-0">
	<Navbar />
	{@render children()}
	<About />
	<Origin />
	<Features />
	<Team />
	<Testimonial />
	<Faqs />
	<Footer />

	
</div>

