<script>
  let { imgSrc='https://thispersondoesnotexist.com/', imgAlt='person', name="Dann the Mann", title="Manager" } = $props();

  // Hover state for animation
  let isHovered = false;

  // Handle hover events
  const handleMouseEnter = () => isHovered = true;
  const handleMouseLeave = () => isHovered = false;
</script>

<div 
  class="w-full sm:w-64 md:w-72 h-80 rounded-lg overflow-hidden shadow-lg transition-all duration-300 hover:shadow-xl bg-white transform hover:-translate-y-1"
  on:mouseenter={handleMouseEnter}
  on:mouseleave={handleMouseLeave}
>
  <div class="relative h-60 overflow-hidden">
      <img 
          src={imgSrc} 
          alt={imgAlt} 
          class="w-full h-full object-cover object-center transition-transform duration-500 {isHovered ? 'scale-110' : 'scale-100'}"
      />
      <!-- Overlay gradient for better text visibility -->
      <div class="absolute inset-0 bg-gradient-to-t from-black/50 to-transparent opacity-0 transition-opacity duration-300 {isHovered ? 'opacity-100' : ''}"></div>
  </div>
  
  <div class="p-4 text-center bg-black h-20 flex flex-col justify-center">
      <h3 class="font-rogBold text-base sm:text-lg font-extrabold text-white truncate">{name}</h3>
      <p class="font-rog text-xs sm:text-sm text-gray-300 mt-1">{title}</p>
  </div>
</div>