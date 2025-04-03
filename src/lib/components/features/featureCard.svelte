<script>
    import Button from '../core/button.svelte'
    let { icon, title= "Web Fuel", description= "When we're not serving coffee, we're fueling the web with custom-built websites.", buttonText="GET STARTED", } = $props();

</script>
  
  <div 
    class="w-96 p-8 flex flex-col items-center justify-center text-center rounded-md bg-transparent"
  >
    <div class="mb-4">
      {#if icon}
         <img class="w-32" src={icon} alt={title}>
      {:else}
          <!-- else content here -->
        <svg width="60" height="60" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M12 1L21 5.5V18.5L12 23L3 18.5V5.5L12 1Z" fill="currentColor" class="text-black" />
          <path d="M18 15L10 19V7L18 11V15Z" fill="currentColor" class="text-black" />
          <path d="M12 4L6 7V11L12 8V4Z" fill="currentColor" class="text-black" />
        </svg>
      {/if}

    </div>
    
    <h2 class="text-4xl font-bold mb-4 text-black">{title}</h2>
    
    <p class="text-black mb-8 max-w-xs">{description}</p>
    <button
            href="#" 
            class="font-rog text-lg bg-white border-[#DC701F] border-2 rounded-xl hover:bg-[#2D1509] text-black hover:text-white font-bold py-2 px-4  transition-all duration-150"
            >
                Shop Coffee Beans
      </button>
  </div>