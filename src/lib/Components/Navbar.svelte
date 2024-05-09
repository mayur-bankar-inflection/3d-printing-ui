<script lang="ts">
	import Icon from '@iconify/svelte';
	import {
		backInOut,
		circInOut,
		elasticInOut,
		quintOut,
		sineIn,
		sineInOut,
		sineOut
	} from 'svelte/easing';
	// import * as Drawer from './ui/drawer';

	import { fly, slide } from 'svelte/transition';

	let isDivVisible = false;

	function toggleDivVisibility() {
		isDivVisible = !isDivVisible;
	}
</script>

<nav class="bg-green-500">
	<div class="mx-auto max-w-7xl sm:px-6 lg:px-8">
		<div class="relative flex h-16 items-center justify-between px-2">
			<div class="sm:hidden">
				<button
					class="rounded-md p-2 text-white hover:bg-white hover:text-cyan-500 focus:outline-none"
					aria-label="Toggle menu"
					on:click={toggleDivVisibility}
				>
					<svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="2"
							d="M4 6h16M4 12h16m-7 6h7"
						></path>
					</svg>
				</button>
				<!-- <Drawer.Trigger class="bg-red-600">Open</Drawer.Trigger> -->
			</div>
			<div
				class="flex flex-1 items-center justify-center p-1 py-2 sm:items-stretch sm:justify-start"
			>
				<div class="hidden flex-shrink-0 items-center md:flex lg:flex">
					<Icon icon="cryptocurrency:beam" width="36" height="36" style="color: #2314f5" />
				</div>
				<div class="hidden sm:ml-6 sm:block">
					<div class="m-1 flex space-x-4">
						<div class="mx-auto content-center rounded-md px-3 py-2 hover:bg-white">
							<a
								href="#"
								class="rounded-md px-3 py-2 text-sm font-medium text-white hover:bg-white hover:text-cyan-500"
							>
								<svg
									class="mx-auto h-6 w-6 text-center text-white hover:text-cyan-500"
									width="20"
									height="20"
									viewBox="0 0 24 24"
									stroke-width="2"
									stroke="currentColor"
									fill="none"
									stroke-linecap="round"
									stroke-linejoin="round"
								>
									<path stroke="none" d="M0 0h24v24H0z" /> <circle cx="12" cy="13" r="2" />
									<line x1="13.45" y1="11.55" x2="15.5" y2="9.5" />
									<path d="M6.4 20a9 9 0 1 1 11.2 0Z" /></svg
								>
								<p>Dashboard</p>
							</a>
						</div>
						<div class="mx-auto content-center rounded-md px-3 py-2 hover:bg-white">
							<a
								href="#"
								class="rounded-md px-3 py-2 text-sm font-medium text-white hover:bg-white hover:text-cyan-500"
							>
								<svg
									class="mx-auto h-6 w-6 text-center text-white hover:text-cyan-500"
									viewBox="0 0 24 24"
									fill="none"
									stroke="currentColor"
									stroke-width="2"
									stroke-linecap="round"
									stroke-linejoin="round"
								>
									<path d="M21.21 15.89A10 10 0 1 1 8 2.83" />
									<path d="M22 12A10 10 0 0 0 12 2v10z" /></svg
								>
								<p>Parts</p>
							</a>
						</div>
						<div class="mx-auto content-center rounded-md px-3 py-2 hover:bg-white">
							<a
								href="#"
								class="rounded-md px-3 py-2 text-sm font-medium text-white hover:bg-white hover:text-cyan-500"
							>
								<svg
									class="mx-auto h-6 w-6 text-center text-white hover:text-cyan-500"
									width="24"
									height="24"
									viewBox="0 0 24 24"
									stroke-width="2"
									stroke="currentColor"
									fill="none"
									stroke-linecap="round"
									stroke-linejoin="round"
								>
									<path stroke="none" d="M0 0h24v24H0z" />
									<polyline points="3 17 9 11 13 15 21 7" />
									<polyline points="14 7 21 7 21 14" /></svg
								>
								<p>Estimation</p>
							</a>
						</div>
					</div>
				</div>
			</div>
			<div
				class="absolute inset-y-0 right-0 m-2 flex items-center pr-2 sm:static sm:inset-auto sm:ml-6 sm:pr-0"
			>
				<div class="mx-auto content-center rounded-md hover:bg-white">
					<a
						href="#"
						class="rounded-md px-3 py-2 text-sm font-medium text-white hover:bg-white hover:text-cyan-500"
					>
						<svg
							class="mx-auto h-6 w-6 text-center text-white hover:text-cyan-500"
							width="24"
							height="24"
							viewBox="0 0 24 24"
							stroke-width="2"
							stroke="currentColor"
							fill="none"
							stroke-linecap="round"
							stroke-linejoin="round"
						>
							<path stroke="none" d="M0 0h24v24H0z" />
							<path
								d="M10.325 4.317c.426-1.756 2.924-1.756 3.35 0a1.724 1.724 0 0 0 2.573 1.066c1.543-.94 3.31.826 2.37 2.37a1.724 1.724 0 0 0 1.065 2.572c1.756.426 1.756 2.924 0 3.35a1.724 1.724 0 0 0 -1.066 2.573c.94 1.543-.826 3.31-2.37 2.37a1.724 1.724 0 0 0 -2.572 1.065c-.426 1.756-2.924 1.756-3.35 0a1.724 1.724 0 0 0 -2.573 -1.066c-1.543.94-3.31-.826-2.37-2.37a1.724 1.724 0 0 0 -1.065 -2.572c-1.756-.426-1.756-2.924 0-3.35a1.724 1.724 0 0 0 1.066 -2.573c-.94-1.543.826-3.31 2.37-2.37.996.608 2.296.07 2.572-1.065z"
							/> <circle cx="12" cy="12" r="3" /></svg
						>
						<p>Setting</p>
					</a>
				</div>
				<div class="m-1 mx-auto content-center rounded-md px-3 py-2 hover:bg-white">
					<a
						href="#"
						class="rounded-md px-3 py-2 text-sm font-medium text-white hover:bg-white hover:text-cyan-500"
					>
						<svg
							class="mx-auto h-6 w-6 text-center text-white hover:text-cyan-500"
							width="24"
							height="24"
							viewBox="0 0 24 24"
							stroke-width="2"
							stroke="currentColor"
							fill="none"
							stroke-linecap="round"
							stroke-linejoin="round"
						>
							<path stroke="none" d="M0 0h24v24H0z" /> <circle cx="12" cy="12" r="9" />
							<line x1="12" y1="17" x2="12" y2="17.01" />
							<path d="M12 13.5a1.5 1.5 0 0 1 1 -1.5a2.6 2.6 0 1 0 -3 -4" /></svg
						>
						<p>Help</p>
					</a>
				</div>

				<div class="relative ml-3">
					<div>
						<button
							type="button"
							class="relative flex rounded-full text-sm focus:outline-none focus:ring-2 focus:ring-white focus:ring-offset-2 focus:ring-offset-gray-800"
							id="user-menu-button"
							aria-expanded="false"
							aria-haspopup="true"
						>
							<svg
								class="h-12 w-12 text-white hover:text-cyan-900"
								fill="none"
								viewBox="0 0 24 24"
								stroke="currentColor"
							>
								<path
									stroke-linecap="round"
									stroke-linejoin="round"
									stroke-width="2"
									d="M5.121 17.804A13.937 13.937 0 0112 16c2.5 0 4.847.655 6.879 1.804M15 10a3 3 0 11-6 0 3 3 0 016 0zm6 2a9 9 0 11-18 0 9 9 0 0118 0z"
								/>
							</svg>
						</button>
					</div>
				</div>
			</div>
		</div>
	</div>

	{#if isDivVisible}
		<div
			class="fixed left-0 top-0 z-50 flex h-full w-full bg-black bg-opacity-50 transition-opacity duration-500"
		>
			<!-- <div
			class="fixed left-0 top-0 z-50 flex h-full w-full items-center justify-center bg-black bg-opacity-50 transition-opacity duration-500"
		> -->
			<!-- class="relative h-full w-[40%] -translate-x-full transform bg-cyan-500 transition-transform duration-500 ease-in-out" -->
			<div
				class="relative h-full w-[40%] bg-green-500"
				transition:slide={{ delay: 200, duration: 500, easing: quintOut, axis: 'x' }}
			>
				<button
					class="absolute right-0 top-0 m-2 flex rounded p-2 text-white hover:bg-white hover:text-cyan-500"
					on:click={toggleDivVisibility}
				>
					<svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="2"
							d="M6 18L18 6M6 6l12 12"
						></path>
					</svg>
				</button>

				<div class="mt-[4rem] space-y-1 px-2 pb-3 pt-2">
					<a
						href="#"
						class="mx-auto block rounded-md px-3 py-2 text-center text-base font-medium text-white hover:bg-white hover:text-cyan-500"
						>Dashboard</a
					>
					<a
						href="#"
						class="mx-auto block rounded-md px-3 py-2 text-center text-base font-medium text-white hover:bg-white hover:text-cyan-500"
						>Parts</a
					>
					<a
						href="#"
						class="mx-auto block rounded-md px-3 py-2 text-center text-base font-medium text-white hover:bg-white hover:text-cyan-500"
						>Estimation</a
					>
				</div>
			</div>
		</div>
	{/if}
</nav>
