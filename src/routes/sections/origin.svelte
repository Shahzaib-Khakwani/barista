<script>
    import { base } from '$app/paths';

</script>

<div class="bg-white min-h-screen w-full relative p-4 sm:p-8 md:p-16">
    <div class="absolute -top-16 sm:-top-20 md:-top-28 left-0 custom-shape-divider-bottom-1743707047">
        <svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none">
            <path d="M985.66,92.83C906.67,72,823.78,31,743.84,14.19c-82.26-17.34-168.06-16.33-250.45.39-57.84,11.73-114,31.07-172,41.86A600.21,600.21,0,0,1,0,27.35V120H1200V95.8C1132.19,118.92,1055.71,111.31,985.66,92.83Z" class="shape-fill"></path>
        </svg>
    </div>

    <div class="flex flex-col-reverse md:flex-row justify-center items-center">
        <div class="w-full md:w-1/2 px-2 sm:px-4 md:px-8 flex justify-center md:justify-end mt-8 md:mt-0">
            <img 
            class="h-64 sm:h-80 md:h-[70vh] rounded-3xl object-cover"
            src="{base}/coffe.webp" 
            alt="coffee">
        </div>
        <div class="w-full md:w-1/2 text-center md:text-left">
            <h1 class="font-rogBold font-extrabold text-4xl sm:text-5xl md:text-6xl lg:text-8xl text-black tracking-tight">
                Organic, Single Origin & Dann Good
            </h1>
            <p class="w-full md:w-5/6 px-0 md:px-4 mt-4 md:mt-8 text-black font-rog mb-6 md:mb-8 text-sm leading-loose">
                Experience the rich flavors of our unique coffee blends, crafted with the finest organic ingredients from around the world. Each sip is a journey to the heart of dann goodness.
            </p>        
            <button
            class="font-rog text-base md:text-lg bg-transparent border-[#DC701F] border-2 rounded-xl hover:bg-[#DC701F] text-black hover:text-white font-bold py-2 px-4 transition-all duration-150"
            >
                Shop Coffee Beans
            </button>
        </div>
    </div>
</div>

<style>
.custom-shape-divider-bottom-1743707047 {
 width: 100%;
 overflow: hidden;
 line-height: 0;
}

.custom-shape-divider-bottom-1743707047 svg {
 position: relative;
 display: block;
 width: calc(180% + 1.3px);
 height: 116px;
 transform: rotateY(180deg);
}

.custom-shape-divider-bottom-1743707047 .shape-fill {
 fill: #FFFFFF;
}
</style>