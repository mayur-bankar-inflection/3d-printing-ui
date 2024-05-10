<script lang="ts">
	let isMenuOpen = false;
	let isButtonClick = false;

	function toggleMenu() {
		isButtonClick = !isButtonClick;
		isMenuOpen = !isMenuOpen;
	}

	function Menu(e: any) {
		e.name === 'menu' ? (e.name = 'close') : (e.name = 'menu');
	}
</script>

<nav class=" navbar-center bg-blue-400 relative h-auto">
	<div class="flex items-center justify-between px-3">
		<a href="/">
			<img src="logo.webp" alt="" class="max-w-[65px] p-1" />
		</a>

		<div class="flex justify-between items-center flex-1 hidden md:flex">
			<div class="flex items-center">
				<a href="/dashboard">
					<div class="tooltip tooltip-bottom" data-tip="dashboard">
						<button
							class="ml-2 w-20 rounded-xl hover:bg-white hover:bg-opacity-55 text-white hover:text-black font-medium duration-300 px-1 py-1"
							aria-current="page"
						>
							<svg
								class="h-6 w-6 mx-auto text-center"
								width="12"
								height="12"
								viewBox="0 0 24 24"
								stroke-width="2"
								stroke="currentColor"
								fill="none"
								stroke-linecap="round"
								stroke-linejoin="round"
							>
								<path stroke="none" d="M0 0h24v24H0z" /> <circle cx="12" cy="13" r="2" />
								<line x1="13.45" y1="11.55" x2="15.5" y2="9.5" />
								<path d="M6.4 20a9 9 0 1 1 11.2 0Z" />
							</svg>
							<p class=" text-xs">Dashboard</p>
						</button>
					</div>
				</a>

				<a href="/">
					<div class="tooltip tooltip-bottom" data-tip="Parts">
						<button
							class="rounded-xl w-20 hover:bg-white hover:bg-opacity-55 text-white hover:text-black duration-300 px-1 py-1"
						>
							<svg
								class="h-6 w-6 mx-auto text-center"
								width="12"
								height="12"
								viewBox="0 0 24 24"
								stroke-width="2"
								stroke="currentColor"
								fill="none"
								stroke-linecap="round"
								stroke-linejoin="round"
							>
								<path
									d="M4 4m0 2a2 2 0 0 1 2 -2h12a2 2 0 0 1 2 2v12a2 2 0 0 1 -2 2h-12a2 2 0 0 1 -2 -2z"
								/>
								<path d="M4 13h3l3 3h4l3 -3h3" />
							</svg>
							<p class="text-xs">Parts</p>
						</button>
					</div>
				</a>

				<a href="/">
					<div class="tooltip tooltip-bottom" data-tip="Estimation">
						<button
							class=" rounded-xl w-20 hover:bg-white hover:bg-opacity-55 text-white hover:text-black duration-300 px-1 py-1"
						>
							<svg
								class="h-6 w-6 mx-auto text-center"
								width="12"
								height="12"
								viewBox="0 0 24 24"
								stroke-width="2"
								stroke="currentColor"
								fill="none"
								stroke-linecap="round"
								stroke-linejoin="round"
							>
								<path d="M4 16l6 -7l5 5l5 -6"></path>
								<path d="M15 14m-1 0a1 1 0 1 0 2 0a1 1 0 1 0 -2 0"></path>
								<path d="M10 9m-1 0a1 1 0 1 0 2 0a1 1 0 1 0 -2 0"></path>
								<path d="M4 16m-1 0a1 1 0 1 0 2 0a1 1 0 1 0 -2 0"></path>
								<path d="M20 8m-1 0a1 1 0 1 0 2 0a1 1 0 1 0 -2 0"></path>
							</svg>
							<p class="text-xs">Estimation</p>
						</button>
					</div>
				</a>
			</div>

			<div class="flex items-center">
				<a href="/">
					<div class="tooltip tooltip-bottom" data-tip="Settings">
						<button
							class=" rounded-xl w-20 hover:bg-white hover:bg-opacity-55 text-white hover:text-black duration-300 px-1 py-1"
						>
							<div>
								<svg
									class="h-6 w-6 mx-auto text-center"
									width="12"
									height="12"
									viewBox="0 0 24 24"
									stroke-width="2"
									stroke="currentColor"
									fill="none"
									stroke-linecap="round"
									stroke-linejoin="round"
								>
									<path d="M14 6m-2 0a2 2 0 1 0 4 0a2 2 0 1 0 -4 0"></path>
									<path d="M4 6l8 0"></path>
									<path d="M16 6l4 0"></path>
									<path d="M8 12m-2 0a2 2 0 1 0 4 0a2 2 0 1 0 -4 0"></path>
									<path d="M4 12l2 0"></path>
									<path d="M10 12l10 0"></path>
									<path d="M17 18m-2 0a2 2 0 1 0 4 0a2 2 0 1 0 -4 0"></path>
									<path d="M4 18l11 0"></path>
									<path d="M19 18l1 0"></path>
								</svg>
								<p class=" text-xs">Settings</p>
							</div>
						</button>
					</div>
				</a>

				<a href="/" class="">
					<div class="tooltip tooltip-bottom" data-tip="Help">
						<button
							class=" w-20 rounded-xl mx-auto hover:bg-white hover:bg-opacity-55 text-white hover:text-black duration-300 px-2 py-1"
							aria-current="page"
						>
							<svg
								class="h-6 w-6 mx-auto text-center"
								width="12"
								height="12"
								viewBox="0 0 24 24"
								stroke-width="2"
								stroke="currentColor"
								fill="none"
								stroke-linecap="round"
								stroke-linejoin="round"
							>
								<path d="M12 12m-4 0a4 4 0 1 0 8 0a4 4 0 1 0 -8 0"></path>
								<path d="M12 12m-9 0a9 9 0 1 0 18 0a9 9 0 1 0 -18 0"></path>
								<path d="M15 15l3.35 3.35"></path>
								<path d="M9 15l-3.35 3.35"></path>
								<path d="M5.65 5.65l3.35 3.35"></path>
								<path d="M18.35 5.65l-3.35 3.35"></path>
							</svg>
							<p class=" text-xs">Help</p>
						</button>
					</div>
				</a>

				<!-- Profile icon -->
				<div class="dropdown dropdown-end mr-1">
					<button class="ml-1">
						<svg
							height="50"
							width="50"
							version="1.1"
							id="Layer_1"
							xmlns="http://www.w3.org/2000/svg"
							xmlns:xlink="http://www.w3.org/1999/xlink"
							viewBox="0 0 512 512"
							xml:space="preserve"
						>
							<path
								style="fill:#FFFFFF;"
								d="M256,508C117.04,508,4,394.96,4,256S117.04,4,256,4s252,113.04,252,252S394.96,508,256,508z"
							/>
							<path
								style="fill:#D6D6D6;"
								d="M256,8c136.752,0,248,111.248,248,248S392.752,504,256,504S8,392.752,8,256S119.248,8,256,8 M256,0	C114.608,0,0,114.608,0,256s114.608,256,256,256s256-114.608,256-256S397.392,0,256,0L256,0z"
							/>
							<g>
								<ellipse style="fill:#0BA4E0;" cx="256" cy="175.648" rx="61.712" ry="60.48" />
								<path
									style="fill:#0BA4E0;"
									d="M362.592,360.624c0-57.696-47.728-104.464-106.592-104.464s-106.592,46.768-106.592,104.464H362.592
		z"
								/>
							</g>
						</svg>
					</button>

					<!-- after click options -->
					<ul class="menu dropdown-content mt-3 z-[1] p-2 shadow bg-base-100 rounded-box w-52">
						<li>
							<a href="/" class="">
								<button class="flex items-center">
									<span class="chakra-menu__icon-wrapper css-7halv9">
										<svg
											xmlns="http://www.w3.org/2000/svg"
											width="16"
											height="16"
											viewBox="0 0 24 24"
											fill="none"
											stroke="currentColor"
											stroke-width="2"
											stroke-linecap="round"
											stroke-linejoin="round"
											class="tabler-icon tabler-icon-receipt-2 chakra-menu__icon"
											focusable="false"
											aria-hidden="true"
											><path
												d="M5 21v-16a2 2 0 0 1 2 -2h10a2 2 0 0 1 2 2v16l-3 -2l-2 2l-2 -2l-2 2l-2 -2l-3 2"
											></path><path
												d="M14 8h-2.5a1.5 1.5 0 0 0 0 3h1a1.5 1.5 0 0 1 0 3h-2.5m2 0v1.5m0 -9v1.5"
											></path></svg
										></span
									><span class="ml-2">Plans and pricing</span></button
								>
							</a>
						</li>
						<li>
							<a href="/">
								<button class="flex items-center">
									<span>
										<svg
											xmlns="http://www.w3.org/2000/svg"
											width="16"
											height="16"
											viewBox="0 0 24 24"
											fill="none"
											stroke="currentColor"
											stroke-width="2"
											stroke-linecap="round"
											stroke-linejoin="round"
											class="tabler-icon tabler-icon-info-circle chakra-menu__icon"
											focusable="false"
											aria-hidden="true"
											><path d="M3 12a9 9 0 1 0 18 0a9 9 0 0 0 -18 0"></path><path d="M12 9h.01"
											></path><path d="M11 12h1v4h1"></path></svg
										></span
									><span class="ml-2">About</span></button
								></a
							>
						</li>
						<hr aria-orientation="horizontal" />

						<li>
							<a href="/">
								<button class="flex items-center">
									<span>
										<svg
											xmlns="http://www.w3.org/2000/svg"
											width="16"
											height="16"
											viewBox="0 0 24 24"
											fill="none"
											stroke="currentColor"
											stroke-width="2"
											stroke-linecap="round"
											stroke-linejoin="round"
											class="tabler-icon tabler-icon-logout chakra-menu__icon"
											focusable="false"
											aria-hidden="true"
											><path
												d="M14 8v-2a2 2 0 0 0 -2 -2h-7a2 2 0 0 0 -2 2v12a2 2 0 0 0 2 2h7a2 2 0 0 0 2 -2v-2"
											></path><path d="M9 12h12l-3 -3"></path><path d="M18 15l3 -3"></path></svg
										></span
									><span class="ml-2">Login</span></button
								></a
							>
						</li>
					</ul>
				</div>
			</div>
		</div>

		<!-- Hamburger menu for small devices -->
		<button tabindex="0" class="md:hidden cursor-pointer" on:click={toggleMenu}>
			{#if isButtonClick}
				<svg
					class="mr-2"
					xmlns="http://www.w3.org/2000/svg"
					xmlns:xlink="http://www.w3.org/1999/xlink"
					fill="#000000"
					height="20"
					width="20"
					version="1.1"
					id="Layer_1"
					viewBox="0 0 512 512"
					xml:space="preserve"
				>
					<g>
						<g>
							<polygon
								points="512,59.076 452.922,0 256,196.922 59.076,0 0,59.076 196.922,256 0,452.922 59.076,512 256,315.076 452.922,512     512,452.922 315.076,256   "
							/>
						</g>
					</g>
				</svg>
			{:else}
				<svg
				class="mr-2 "
					width="30"
					height="30"
					viewBox="0 0 24 24"
					fill="none"
					xmlns="http://www.w3.org/2000/svg"
				>
					<path d="M4 18L20 18" stroke="#000000" stroke-width="2" stroke-linecap="round" />
					<path d="M4 12L20 12" stroke="#000000" stroke-width="2" stroke-linecap="round" />
					<path d="M4 6L20 6" stroke="#000000" stroke-width="2" stroke-linecap="round" />
				</svg>
			{/if}
		</button>
	</div>
	<!-- hamburger menu contents for small devices -->
	<div class="md:hidden bg-white rounded-sm p-0">
		<ul
			class:open={isMenuOpen}
			class=" font-semibold px-2 py-3 cursor-pointer transition-all ease-in duration-500"
		>
			<li class="mb-2 hover:bg-slate-200 duration-300 rounded-md p-2">
				<a href="/">Dashboard</a>
			</li>
			<li class="mb-2 hover:bg-slate-200 duration-300 rounded-md p-2">
				<a href="/">Parts</a>
			</li>
			<li class="mb-2 hover:bg-slate-200 duration-300 rounded-md p-2">
				<a href="/">Estimation</a>
			</li>
			<li class="mb-2 hover:bg-slate-200 duration-300 rounded-md p-2">
				<a href="/">Settings</a>
			</li>
			<li class="mb-2 hover:bg-slate-200 duration-300 rounded-md p-2">
				<a href="/">Help</a>
			</li>
		</ul>
		<hr>
	</div>
</nav>
