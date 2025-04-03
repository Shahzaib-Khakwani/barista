<script>
    import { base } from "$app/paths";

    const logoSrc = `${base}/logo.svg`;
    const logoAlt = "Dann Good Coffee";
    
    let mobileMenuOpen = $state(false);
    
    const toggleMobileMenu = () => {
      mobileMenuOpen = !mobileMenuOpen;
    };
    
    const menuItems = [
      { name: "MENU", href: "/menu" },
      { name: "SHOP", href: "/shop" },
      { name: "ABOUT", href: "/about" }
    ];
  </script>
  <nav class="absolute top-0 left-0 w-full bg-transparent z-10">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex justify-between items-center h-16 lg:h-20">
        <!-- Left menu items (desktop) -->
        <div class="hidden md:flex items-center space-x-8">
          {#each menuItems as item}
            <a href={item.href} class="text-white font-bold hover:text-orange-400 transition-colors">
              {item.name}
            </a>
          {/each}
        </div>
        
        <!-- Mobile menu button -->
        <div class="md:hidden flex items-center">
          <button 
            type="button" 
            class="text-white hover:text-orange-400"
            on:click={toggleMobileMenu}
            aria-label="Toggle menu"
          >
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d={mobileMenuOpen ? "M6 18L18 6M6 6l12 12" : "M4 6h16M4 12h16M4 18h16"} />
            </svg>
          </button>
        </div>
        
        <!-- Logo (center) -->
        <div class="absolute left-1/2 transform -translate-x-1/2">
          <a href="/" class="flex items-center">
            <img src={logoSrc} alt={logoAlt} class="mt-4 h-20 w-auto" />
          </a>
        </div>
        
        <!-- Order button (right) -->
        <div>
          <a 
            href="/order" 
            class="bg-orange-500 hover:bg-orange-600 text-white font-bold py-2 px-4 rounded transition-colors"
          >
            ORDER
          </a>
        </div>
      </div>
    </div>
    
    <!-- Mobile menu (responsive) -->
    {#if mobileMenuOpen}
      <div class="md:hidden bg-gray-900 bg-opacity-95 absolute w-full">
        <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
          {#each menuItems as item}
            <a 
              href={item.href} 
              class="text-white block px-3 py-2 rounded-md text-base font-medium hover:bg-gray-800"
              on:click={() => mobileMenuOpen = false}
            >
              {item.name}
            </a>
          {/each}
        </div>
      </div>
    {/if}
  </nav>