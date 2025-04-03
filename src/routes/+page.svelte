<script>
    import { base } from '$app/paths';
	import FeatureCard from './../lib/components/features/featureCard.svelte';
    import TeamCard from "$lib/components/features/teamCard.svelte";
    import Button from '$lib/components/core/button.svelte';
</script>

<div 
class="min-h-screen w-full relative flex flex-col justify-center items-center px-4 md:px-6" 
style="background-image: url('{base}/hero.png'); background-size: cover; background-position: center;">
    <div class="text-center w-full md:w-4/5 lg:w-3/5">
        <h1 class="font-rogBold font-bold text-4xl sm:text-5xl md:text-6xl lg:text-8xl text-white tracking-tight">
            Chill Vibes and Dann Good Coffee
        </h1>
        <p class="text-white font-rog mb-6 md:mb-8 text-base md:text-lg leading-loose max-w-3xl mx-auto">
            An inspiring space to fuel your ambition and coffee that's dann good.
        </p>
    </div>
    <div class="flex flex-col sm:flex-row justify-center items-center gap-4">
        <Button content='Order' />
        <button
            href="/order" 
            class="font-rog text-base md:text-lg bg-transparent border-white border-2 rounded-xl hover:bg-white text-white hover:text-black font-bold py-2 px-4 w-full sm:w-auto transition-all duration-150"
        >
            Menu
        </button>
    </div>
</div>