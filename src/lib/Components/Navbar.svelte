<script lang="ts">
	import * as Sheet from '$lib/Components/ui/sheet';
	import Button from './ui/button/button.svelte';

	let clickedOption = false;
	function onClickOption() {
		clickedOption = !clickedOption;
	}
</script>

<nav class=" h-fit w-full bg-zinc-800 py-4">
	<div class="mx-auto max-w-7xl sm:px-6 lg:px-8">
		<div class="relative flex h-16 w-full items-center justify-between px-2">
			<div class=" sm:hidden">
				<Sheet.Root>
					<Sheet.Trigger asChild let:builder>
						<Button builders={[builder]} variant="outline"
							><svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
								<path
									stroke-linecap="round"
									stroke-linejoin="round"
									stroke-width="2"
									d="M4 6h16M4 12h16m-7 6h7"
								></path>
							</svg></Button
						>
					</Sheet.Trigger>
					<Sheet.Content side="left" class="space-y-2">
						<Button class=""
							><img
								src="/Navbar/acc.png"
								alt="Account Icon"
								class="mx-auto block h-8 w-8 rounded-md"
							/></Button
						>
						<Sheet.Close asChild let:builder>
							<Button
								href="/"
								builders={[builder]}
								class=" mx-auto   block rounded-md px-3 py-2 text-center text-base font-medium hover:bg-yellow-500 hover:text-zinc-950 "
								>Home</Button
							>
						</Sheet.Close>

						<Sheet.Close asChild let:builder>
							<Button
								builders={[builder]}
								href="/dashboard"
								class=" mx-auto   block rounded-md px-3 py-2 text-center text-base font-medium hover:bg-yellow-500 hover:text-zinc-950 "
								>Dashboard</Button
							>
						</Sheet.Close>

						<Sheet.Close asChild let:builder>
							<Button
								builders={[builder]}
								href="/estimation"
								class=" mx-auto   block rounded-md px-3 py-2 text-center text-base font-medium hover:bg-yellow-500 hover:text-zinc-950 "
								>Estimation</Button
							>
						</Sheet.Close>

						<Sheet.Close asChild let:builder>
							<Button
								builders={[builder]}
								href="/help"
								class=" mx-auto block rounded-md px-3 py-2 text-center text-base font-medium hover:bg-yellow-500 hover:text-zinc-950 "
								>Help</Button
							>
						</Sheet.Close>
					</Sheet.Content>
				</Sheet.Root>
			</div>
			<div
				class="flex flex-1 items-center justify-center p-1 py-2 sm:items-stretch sm:justify-start"
			>
				<div class="hidden flex-shrink-0 items-center md:flex lg:flex lg:space-x-6">
					<img src="apexlogo.svg" alt="" class="h-36 w-36" />
					<a href="/">
						<button
							class="rounded-md px-3 py-3 text-sm font-medium text-white hover:bg-yellow-500 hover:text-white"
						>
							<svg
								class="mx-auto h-8 w-8 text-white"
								fill="none"
								viewBox="0 0 24 24"
								stroke="currentColor"
							>
								<path
									stroke-linecap="round"
									stroke-linejoin="round"
									stroke-width="2"
									d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6"
								/>
							</svg>

							Home
						</button>
					</a>
					<a href="/dashboard">
						<button
							class="rounded-md px-3 py-3 text-sm font-medium text-white hover:bg-yellow-500 hover:text-white"
						>
							<svg
								class="mx-auto h-7 w-7 text-center"
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

							Dashboard
						</button>
					</a>
					<a href="/estimation">
						<button
							class="rounded-md px-3 py-3 text-sm font-medium text-white hover:bg-yellow-500 hover:text-white"
						>
							<svg
								class="mx-auto h-7 w-7 text-center"
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

							Estimation
						</button>
					</a>
				</div>
			</div>

			<div class=" hidden flex-shrink-0 flex-row items-center sm:flex md:flex lg:flex">
				<a href="/help">
					<button
						class="rounded-md px-3 py-3 text-sm font-medium text-white hover:bg-yellow-500 hover:text-white"
					>
						<svg
							class="mx-auto h-7 w-7 text-center"
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
						Help
					</button>
				</a>
			</div>
			<div class="ml-6 sm:flex">
				<div>
					<button
						type="button"
						class="relative flex rounded-full text-sm focus:outline-none focus:ring-2 focus:ring-white focus:ring-offset-2 focus:ring-offset-gray-800"
						id="user-menu-button"
						aria-expanded="false"
						aria-haspopup="true"
					>
						<svg class="h-14 w-14 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="1"
								d="M5.121 17.804A13.937 13.937 0 0112 16c2.5 0 4.847.655 6.879 1.804M15 10a3 3 0 11-6 0 3 3 0 016 0zm6 2a9 9 0 11-18 0 9 9 0 0118 0z"
							/>
						</svg>
					</button>
				</div>
			</div>
		</div>
	</div>
</nav>
