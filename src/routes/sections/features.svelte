<script>
    import { base } from "$app/paths";

    import FeatureCard from "$lib/components/features/featureCard.svelte";
</script>

<div class="bg-[#c06522] min-h-[60vh] w-full relative p-4 sm:p-8 md:p-16">
    <div class="absolute left-0 -top-12 sm:-top-16 md:-top-20 custom-shape-divider-bottom-1743709570">
        <svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none">
            <path d="M985.66,92.83C906.67,72,823.78,31,743.84,14.19c-82.26-17.34-168.06-16.33-250.45.39-57.84,11.73-114,31.07-172,41.86A600.21,600.21,0,0,1,0,27.35V120H1200V95.8C1132.19,118.92,1055.71,111.31,985.66,92.83Z" class="shape-fill"></path>
        </svg>
    </div>
    <div class="flex flex-col sm:flex-row justify-center items-center gap-6 sm:gap-4">
        <FeatureCard title="Custom Roasts" icon='{base}/coffeeBeans.svg' />
        <FeatureCard title="Training" icon='{base}/arrow.svg' />
        <FeatureCard title="Custom Roasts" icon='{base}/coffeeBeans.svg' />
    </div>
</div>

<style>
.custom-shape-divider-bottom-1743709570 {
    width: 100%;
    overflow: hidden;
    line-height: 0;
}

.custom-shape-divider-bottom-1743709570 svg {
    position: relative;
    display: block;
    width: calc(100% + 1.3px);
    height: 93px;
}

.custom-shape-divider-bottom-1743709570 .shape-fill {
    fill: #C06522;
}
</style>