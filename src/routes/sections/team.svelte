<script>
    import TeamCard from "$lib/components/features/teamCard.svelte";
</script>

<div class="bg-white min-h-[60vh] w-full relative p-4 sm:p-8 md:p-16">
    <div class="absolute -top-0 left-0 custom-shape-divider-top-1743711259">
        <svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none">
            <path d="M0,0V46.29c47.79,22.2,103.59,32.17,158,28,70.36-5.37,136.33-33.31,206.8-37.5C438.64,32.43,512.34,53.67,583,72.05c69.27,18,138.3,24.88,209.4,13.08,36.15-6,69.85-17.84,104.45-29.34C989.49,25,1113-14.29,1200,52.47V0Z" opacity=".25" class="shape-fill"></path>
            <path d="M0,0V15.81C13,36.92,27.64,56.86,47.69,72.05,99.41,111.27,165,111,224.58,91.58c31.15-10.15,60.09-26.07,89.67-39.8,40.92-19,84.73-46,130.83-49.67,36.26-2.85,70.9,9.42,98.6,31.56,31.77,25.39,62.32,62,103.63,73,40.44,10.79,81.35-6.69,119.13-24.28s75.16-39,116.92-43.05c59.73-5.85,113.28,22.88,168.9,38.84,30.2,8.66,59,6.17,87.09-7.5,22.43-10.89,48-26.93,60.65-49.24V0Z" opacity=".5" class="shape-fill"></path>
            <path d="M0,0V5.63C149.93,59,314.09,71.32,475.83,42.57c43-7.64,84.23-20.12,127.61-26.46,59-8.63,112.48,12.24,165.56,35.4C827.93,77.22,886,95.24,951.2,90c86.53-7,172.46-45.71,248.8-84.81V0Z" class="shape-fill"></path>
        </svg>
    </div>
    <div class="flex flex-col space-y-8 md:space-y-16 justify-center items-center">
        <h1 class="z-30 font-rogBold font-bold text-4xl sm:text-5xl md:text-6xl lg:text-8xl text-black tracking-tight text-center">
            Meet Our Team
        </h1>
        <div class="flex flex-col sm:flex-row flex-wrap justify-center items-center gap-6 sm:gap-4 md:gap-6 lg:gap-8">
            <TeamCard />
            <TeamCard />
            <TeamCard />
            <TeamCard />
        </div>
    </div>
</div>

<style>
.custom-shape-divider-top-1743711259 {
    width: 100%;
    overflow: hidden;
    line-height: 0;
}

.custom-shape-divider-top-1743711259 svg {
    position: relative;
    display: block;
    width: calc(100% + 1.3px);
    height: 93px;
}

.custom-shape-divider-top-1743711259 .shape-fill {
    fill: #C06522;
}
</style>