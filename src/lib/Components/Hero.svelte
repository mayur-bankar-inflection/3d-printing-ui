<script lang="ts">
	import Button from './ui/button/button.svelte';
	import { Input } from '$lib/components/ui/input/index.js';
	import { Label } from '$lib/components/ui/label/index.js';
</script>

<section class="relative flex h-[645px] flex-col justify-center text-left text-white">
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
	<!-- Your video content -->
	<div
		class="video-content font-Onest z-10 flex flex-col justify-center space-y-2 px-12 md:text-center lg:items-start lg:px-8 xl:mx-8"
	>
		<h1 class="animate__animated animate__fadeInUp text-4xl font-semibold lg:px-0 lg:text-6xl">
			Enhance Manufacturing
		</h1>
		<h1 class="animate__animated animate__fadeInUp text-4xl font-semibold lg:text-6xl">
			With <span class=" font-bold text-yellow-500">3D PRINTING</span>
		</h1>
		<h3 class="animate__animated animate__fadeInUp px-2 text-lg font-light lg:text-2xl">
			Unlock the full potential of additive manufacturing for your business
		</h3>
	</div>

	<!-- Sign-up form for large screen and above -->
	<div
		class="inset-0 z-50 my-5 flex items-center justify-center lg:absolute lg:my-0 lg:justify-end lg:px-10"
	>
		<form
			class="d w-3/4 rounded-xl bg-white bg-opacity-60 px-5 py-5 shadow-md md:w-1/3 lg:w-1/4 lg:px-10 xl:mx-8 xl:py-8"
		>
			<h2 class="mb-4 text-center text-3xl font-semibold text-zinc-800 md:text-4xl">Sign in</h2>
			<div class="mb-4">
				<Label class="mb-1 block text-lg  font-semibold text-zinc-800" for="email">Email</Label>
				<Input
					class=" w-full appearance-none rounded border  leading-tight text-gray-700 focus:outline-none"
					id="email"
					type="email"
					placeholder="abc@gmail.com"
					required
				/>
			</div>
			<div class="mb-4">
				<Label class="mb-1 block text-lg font-semibold text-zinc-800" for="password">
					Password
				</Label>
				<Input
					class="focus:shadow-outline w-full appearance-none rounded border px-5 py-4 leading-tight text-gray-700 focus:outline-none"
					id="password"
					type="password"
					placeholder="Enter your password"
				/>
			</div>
			<!-- Add more form fields as needed -->
			<div class="flex w-full items-center justify-center">
				<Button
					class=" w-full max-w-xs rounded bg-zinc-800 px-4 py-2 font-bold text-white hover:bg-black"
				>
					login
				</Button>
			</div>
			<!-- <p>OR</p> -->
			<div class="mt-4 flex items-center justify-center">
				<Button
					class="flex w-full max-w-xs gap-2 rounded-lg border bg-white px-8 py-2 text-zinc-800 hover:bg-slate-300  "
				>
					<img
						class="h-6 w-6"
						src="https://www.svgrepo.com/show/475656/google-color.svg"
						loading="lazy"
						alt="google logo"
					/>
					<span class=" font-semibold">Login with Google</span>
				</Button>
			</div>
		</form>
	</div>
	<!-- End of sign-up form -->
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
