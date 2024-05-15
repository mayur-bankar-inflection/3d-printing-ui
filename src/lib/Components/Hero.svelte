<script>
	import Button from './ui/button/button.svelte';
</script>

<section class="relative flex h-[645px] flex-col justify-center px-4 text-left text-white lg:pl-52">
	<div class="video-docker absolute left-0 top-0 h-full w-full overflow-hidden">
		<!-- Your video code here -->
		<video
			class="absolute min-h-full min-w-full object-cover"
			src="/Hero/printer.mp4"
			autoplay
			muted
			loop
		></video>
	</div>
	<!-- Sign-up form -->
	<div class="absolute inset-0 z-50 mr-44 flex items-center justify-end">
		<form class="max-w-lg rounded-xl bg-white  bg-opacity-60 px-12 py-10 shadow-md hidden xl:block">
			<h2 class="mb-4 text-3xl font-semibold text-zinc-800">Sign in</h2>
			<div class="mb-4">
				<label class="mb-2 block text-base font-semibold text-zinc-800" for="email"> Email </label>
				<input
					class=" w-full appearance-none rounded border px-5 py-2 leading-tight text-gray-700 focus:outline-none"
					id="email"
					type="email"
					placeholder="abc@gmail.com"
                    required
				/>
			</div>
			<div class="mb-4">
				<label class="mb-2 block text-base font-semibold text-zinc-800" for="password">
					Password
				</label>
				<input
					class="focus:shadow-outline w-full appearance-none rounded border px-5 py-2 leading-tight text-gray-700 focus:outline-none"
					id="password"
					type="password"
					placeholder="Enter your password"
				/>
			</div>
			<!-- Add more form fields as needed -->
			<div class="flex w-full items-center justify-center">
				<button
					class=" w-full max-w-xs rounded bg-zinc-800 px-4 py-2 font-bold text-white hover:bg-black"
				>
					login
				</button>
			</div>
            <div class="flex items-center justify-center mt-4">
                <button class="px-8 py-2 max-w-xs bg-white hover:bg-slate-300 border flex gap-2 rounded-lg text-zinc-800  ">
                    <img class="w-6 h-6" src="https://www.svgrepo.com/show/475656/google-color.svg" loading="lazy" alt="google logo">
                    <span class=" font-semibold">Login with Google</span>
                </button>
            </div>
			
		</form>
	</div>
	<!-- End of sign-up form -->
	<!-- Your video content -->
	<div class="video-content font-Onest z-10 space-y-2">
		<h1 class="animate__animated animate__fadeInUp text-4xl font-semibold lg:text-6xl">
			Enhance Manufacturing
		</h1>
		<h1 class="animate__animated animate__fadeInUp text-4xl font-semibold lg:text-6xl">
			With <span class=" font-bold text-yellow-500">3D PRINTING</span>
		</h1>
		<h3 class="animate__animated animate__fadeInUp text-lg font-light lg:text-2xl">
			Unlock the full potential of additive manufacturing for your business
		</h3>
	</div>
</section>

<style>
	.video-docker video {
		top: 50%;
		left: 50%;
		transform: translate(-50%, -50%);
	}
	.video-docker::after {
		content: '';
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		left: 0;
		background: rgba(0, 0, 0, 0.6);
		z-index: 1;
	}
</style>
