<script lang="ts">
  import { Link } from "svelte-routing";
  let isMenuOpen = false;
</script>

<nav class="bg-white shadow-lg">
  <div class="container mx-auto px-4">
    <div class="flex justify-between items-center h-16">
      <div class="flex items-center">
        <Link to="/" class="text-2xl font-bold text-primary-600">Pillarays</Link>
      </div>

      <!-- Desktop Menu -->
      <div class="hidden md:flex items-center space-x-8">
        
        <Link to="/services" class="text-gray-700 hover:text-primary-600">Services</Link>
        <Link to="/about" class="text-gray-700 hover:text-primary-600">About</Link>
        <Link to="/contact" class="text-gray-700 hover:text-primary-600">Contact</Link>
        <Link to="/foundation" class="text-gray-700 hover:text-primary-600">Foundation</Link>
        <a href="#login" class="btn btn-primary">Client Login</a>
      </div>

      <!-- Mobile Menu Button -->
      <button 
        class="md:hidden"
        on:click={() => isMenuOpen = !isMenuOpen}
      >
        <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          {#if isMenuOpen}
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
          {:else}
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
          {/if}
        </svg>
      </button>
    </div>

    <!-- Mobile Menu -->
    {#if isMenuOpen}
      <div class="md:hidden py-4">
        <div class="flex flex-col space-y-4">
          <Link to="/services" class="text-gray-700 hover:text-primary-600">Services</Link>
          <Link to="/about" class="text-gray-700 hover:text-primary-600">About</Link>
          <Link to="/contact" class="text-gray-700 hover:text-primary-600">Contact</Link>
          <Link to="/foundation" class="text-gray-700 hover:text-primary-600">Foundation</Link>
          <a href="#login" class="btn btn-primary text-center">Client Login</a>
        </div>
      </div>
    {/if}
  </div>
</nav>