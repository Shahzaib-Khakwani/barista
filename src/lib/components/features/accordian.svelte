<script>
    export let open = false;
    import { slide } from 'svelte/transition';
    const handleClick = () => open = !open;
  </script>
  
  <div class="accordion">
    <div class="header" on:click={handleClick}>
      <div class="text">
        <slot name="head"></slot>  
      </div>
      
      <button on:click|stopPropagation={handleClick} aria-label={open ? "Close accordion" : "Open accordion"}>
        <svg class="chevron" class:open viewBox="0 0 24 24" width="24" height="24">
          <path d="M7 10l5 5 5-5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" />
        </svg>
      </button>
    </div>
    
    {#if open}
    <div class="details" transition:slide={{duration: 300}}>
      <slot name="details"></slot>
    </div>
    {/if}
  </div>
  
  <style>
    div.accordion {
      margin: 1rem 0;
      border-radius: 12px;
      background-color: #ffffff;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
      overflow: hidden;
      width: 100%;
    }
    
    div.header {
      display: flex;
      width: 100%;
      padding: 1.5rem;
      align-items: center;
      cursor: pointer;
      border-bottom: 1px solid transparent;
      transition: background-color 0.2s;
    }
    
    div.header:hover {
      background-color: #f9f9f9;
    }
    
    div.header .text {
      flex: 1;
      margin-right: 12px;
      font-weight: 700;
      font-size: 1.25rem;
      color: #222222;
    }
    
    button {
      background: none;
      border: none;
      padding: 0.5rem;
      cursor: pointer;
      display: flex;
      align-items: center;
      justify-content: center;
      color: #555555;
      border-radius: 50%;
      width: 35px;
      height: 35px;
      transition: background-color 0.2s;
    }
    
    button:hover {
      background-color: rgba(0, 0, 0, 0.05);
    }
    
    .chevron {
      transition: transform 0.3s ease;
      transform: rotate(0deg);
    }
    
    .chevron.open {
      transform: rotate(180deg);
    }
    
    div.details {
      padding: 1.5rem;
      color: #444444;
      line-height: 1.5;
      background-color: #ffffff;
      border-top: 1px solid #f0f0f0;
    }
  </style>