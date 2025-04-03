<script>
    import { base } from "$app/paths";
    import { fly } from "svelte/transition";
</script>

<div 
class="bg-[#369392] min-h-[80vh] w-full relative p-4 sm:p-8 md:p-16"
>
<!-- divider -->
<div class="absolute -top-28 left-0 custom-shape-divider-bottom-1743705340">
    <svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none">
        <path d="M321.39,56.44c58-10.79,114.16-30.13,172-41.86,82.39-16.72,168.19-17.73,250.45-.39C823.78,31,906.67,72,985.66,92.83c70.05,18.48,146.53,26.09,214.34,3V0H0V27.35A600.21,600.21,0,0,0,321.39,56.44Z" class="shape-fill"></path>
    </svg>
</div>

<!-- Cup image positioned absolutely -->
<img 
    class="absolute -top-48 right-4 h-[120vh] hidden md:block"
    src="{base}/cup.png" 
    alt="cup">

<div class="flex flex-col md:flex-row justify-center items-center">
    <div class="w-full md:w-1/2">
        <h1 class="font-rogBold font-extrabold text-3xl sm:text-5xl md:text-6xl lg:text-8xl text-black tracking-tight">
            Peruse Our Vintage, Mid-Century Vibe
        </h1>
        <p class="w-full md:w-5/6 px-0 md:px-4 mt-4 md:mt-8 text-black font-rog mb-6 md:mb-8 text-sm leading-loose">
            Step into a world of surf, skating, snowboarding, outdoor adventure, and mid-century awesomeness at Dann Good Coffee. Our coffee shop is inspired by the retro vibes of the past, offering a cozy and nostalgic atmosphere for coffee lovers to enjoy.
        </p>        
        <button
        class="font-rog text-base md:text-lg bg-transparent border-black border-2 rounded-xl hover:bg-black text-black hover:text-white font-bold py-2 px-4 transition-all duration-150"
        >
            Read Our Origin Story
        </button>
    </div>
    
    <!-- Mobile-only image -->
    <div class="w-full md:hidden flex justify-center mt-8">
        <img 
            class="h-64 object-contain"
            src="{base}/cup.png" 
            alt="cup">
    </div>
    
    <!-- This div takes up space on desktop but has no content, since the image is absolutely positioned -->
    <div class="hidden md:block w-1/2"></div>
</div>

</div>

<style>
    .custom-shape-divider-bottom-1743705340 {
        width: 100%;
        overflow: hidden;
        line-height: 0;
        transform: rotate(180deg);
    }


    .custom-shape-divider-bottom-1743705340 svg {
        position: relative;
        display: block;
        width: calc(106% + 1.3px);
        height: 119px;
    }

    .custom-shape-divider-bottom-1743705340 .shape-fill {
        fill: #369392;
    }
</style>