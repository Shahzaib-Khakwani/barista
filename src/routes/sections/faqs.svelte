<script>
    import { base } from '$app/paths';
    import Accordion from '$lib/components/features/accordian.svelte';
</script>
  

<div class="bg-[#F4ECE8] min-h-screen w-full relative p-16">
    <div class="absolute -top-0 left-0 custom-shape-divider-top-1743714398">
        <svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none">
            <path d="M321.39,56.44c58-10.79,114.16-30.13,172-41.86,82.39-16.72,168.19-17.73,250.45-.39C823.78,31,906.67,72,985.66,92.83c70.05,18.48,146.53,26.09,214.34,3V0H0V27.35A600.21,600.21,0,0,0,321.39,56.44Z" class="shape-fill"></path>
        </svg>
    </div>
    <div class="max-w-6xl mx-auto">
        <h2 class="font-rogBold text-7xl md:text-6xl font-black text-black mb-16 text-center mb-4">FAQS</h2>
        <div class="w-3/5 mx-auto">

            <Accordion>
                <div slot="head">What is your coffee sourced?</div>
                <div slot="details">
                Our coffee beans are ethically sourced from small-scale farmers in Ethiopia, Colombia, and Costa Rica. We maintain direct trade relationships to ensure fair compensation and sustainable farming practices.
                </div>
            </Accordion>
        
            <Accordion>
                <div slot="head">Do you offer vegan options?</div>
                <div slot="details">
                Yes, we offer a variety of plant-based milk alternatives including oat, almond, soy, and coconut at no extra charge. Our pastry selection also includes several vegan options daily.
                </div>
            </Accordion><Accordion>
                <div slot="head">What is your coffee sourced?</div>
                <div slot="details">
                Our coffee beans are ethically sourced from small-scale farmers in Ethiopia, Colombia, and Costa Rica. We maintain direct trade relationships to ensure fair compensation and sustainable farming practices.
                </div>
            </Accordion>
        
            <Accordion>
                <div slot="head">Do you offer vegan options?</div>
                <div slot="details">
                Yes, we offer a variety of plant-based milk alternatives including oat, almond, soy, and coconut at no extra charge. Our pastry selection also includes several vegan options daily.
                </div>
            </Accordion>
    </div>

    </div>

</div>
<style>
    .custom-shape-divider-top-1743714398 {
    width: 100%;
    overflow: hidden;
    line-height: 0;
}

.custom-shape-divider-top-1743714398 svg {
    position: relative;
    display: block;
    width: calc(100% + 1.3px);
    height: 102px;
}

.custom-shape-divider-top-1743714398 .shape-fill {
    fill: #006764;
}

</style>