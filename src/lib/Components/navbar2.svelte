<script>
	import Icon from '@iconify/svelte';
	import { fade } from 'svelte/transition';

	let isMenuOpen = false;

	function toggleMenu() {
		isMenuOpen = !isMenuOpen;
	}
</script>

<nav class="bg-cyan-500">
	<div class="mx-auto max-w-7xl sm:px-6 lg:px-8">
		<div class="relative flex h-16 px-2 items-center justify-between">
			<div
				class="flex flex-1 items-center justify-center sm:items-stretch sm:justify-start py-2 p-1"
			>
				<div class="flex-shrink-0 items-center hidden md:flex lg:flex">
					<Icon icon="cryptocurrency:beam" width="36" height="36" style="color: #2314f5" />
				</div>
				<div class="hidden sm:ml-6 sm:block">
					<div class="flex space-x-4 m-1">
						<!-- Navbar links -->
						<a href="#" class="nav-link">Dashboard</a>
						<a href="#" class="nav-link">Parts</a>
						<a href="#" class="nav-link">Estimation</a>
					</div>
				</div>
			</div>
			<!-- Menu button for small screens -->
			<div class="sm:hidden">
				<button
					class="text-white p-2 rounded-md focus:outline-none focus:bg-white focus:text-cyan-500"
					aria-label="Toggle menu"
					on:click={toggleMenu}
				>
					<svg class="h-6 w-6 bg-orange-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="2"
							d="M4 6h16M4 12h16m-7 6h7"
						></path>
					</svg>
				</button>
			</div>
		</div>
	</div>

	<!-- Menu drawer for small screens -->
	{#if isMenuOpen}
		<div
			class="fixed inset-0 z-50 flex justify-center items-center bg-black bg-opacity-50"
			in:fade
			
		>
			<div class="bg-white rounded-lg p-4 w-80">
				<a href="#" class="drawer-link block py-2">Dashboard</a>
				<a href="#" class="drawer-link block py-2">Parts</a>
				<a href="#" class="drawer-link block py-2">Estimation</a>
			</div>
		</div>
	{/if}
</nav>


  
  <nav class="bg-cyan-500">
	<div class="mx-auto max-w-7xl sm:px-6 lg:px-8">
	  <div class="relative flex h-16 px-2 items-center justify-between">
		<div class="flex flex-1 items-center justify-center sm:items-stretch sm:justify-start py-2 p-1">
		  <div class="flex-shrink-0 items-center hidden md:flex lg:flex">
			<Icon icon="cryptocurrency:beam" width="36" height="36" style="color: #2314f5" />
		  </div>
		  <div class="hidden sm:ml-6 sm:block">
			<div class="flex space-x-4 m-1">
			  <!-- Navbar links -->
			  <a href="#" class="nav-link">Dashboard</a>
			  <a href="#" class="nav-link">Parts</a>
			  <a href="#" class="nav-link">Estimation</a>
			</div>
		  </div>
		</div>
		<!-- Menu button for small screens -->
		<div class="sm:hidden">
		  <button
			class="text-white p-2 rounded-md focus:outline-none focus:bg-white focus:text-cyan-500"
			aria-label="Toggle menu"
			on:click={toggleMenu}
		  >
			<svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
			  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path>
			</svg>
		  </button>
		</div>
	  </div>
	</div>
  
	<!-- Menu drawer for small screens -->
	<!-- <div class="{ 'translate-x-0': isMenuOpen, 'translate-x-full': !isMenuOpen } fixed inset-y-0 right-0 z-50 flex flex-col justify-center items-center bg-black bg-opacity-50 w-full transition-transform duration-300 ease-in-out">
	  <div class="bg-white rounded-lg p-4 w-80">
		<a href="#" class="drawer-link block py-2">Dashboard</a>
		<a href="#" class="drawer-link block py-2">Parts</a>
		<a href="#" class="drawer-link block py-2">Estimation</a>
	  </div>
	</div> -->
  </nav>
  
  <style>
	/* Define your custom styles here */
	.nav-link {
	  @apply text-white hover:bg-white hover:text-cyan-500 rounded-md px-3 py-2 text-sm font-medium;
	}
  
	.drawer-link {
	  @apply text-black hover:bg-cyan-500 hover:text-white rounded-md px-3 py-2 text-base font-medium;
	}
  </style>
  
