<script lang="ts">
	import Button from './ui/button/button.svelte';
	import { Input } from '$lib/components/ui/input/index.js';
	import { Label } from '$lib/components/ui/label/index.js';
</script>

<section class="relative flex h-[645px] flex-col justify-center  text-left text-white ">
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
		<div class="video-content font-Onest z-10 space-y-2 lg:px-8 flex flex-col justify-center items-center text-center lg:items-start">
			<h1 class="animate__animated animate__fadeInUp text-4xl font-semibold lg:text-6xl  lg:px-0">
				Enhance Manufacturing
			</h1>
			<h1 class="animate__animated animate__fadeInUp text-4xl font-semibold lg:text-6xl ">
				With <span class=" font-bold text-orange-500">3D PRINTING</span>
			</h1>
			<h3 class="animate__animated animate__fadeInUp text-lg font-light lg:text-2xl px-2 ">
				Unlock the full potential of additive manufacturing for your business
			</h3>
		</div>

		<!-- Sign-up form for large screen and above -->
	<div class="lg:absolute inset-0 z-50 lg:px-10 my-5 lg:my-0 flex items-center justify-center lg:justify-end ">
		<form class="rounded-xl w-3/4 lg:w-1/4 bg-white  bg-opacity-60 px-5 lg:px-10 py-5 shadow-md ">
			<h2 class="mb-4 text-4xl text-center font-semibold text-zinc-800">Sign in</h2>
			<div class="mb-4">
				<Label class="mb-1 block text-lg  font-semibold text-zinc-800" for="email"> Email </Label>
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
            <div class="flex items-center justify-center mt-4">
                <Button class="w-full px-8 py-2 max-w-xs bg-white hover:bg-slate-300 border flex gap-2 rounded-lg text-zinc-800  ">
                    <img class="w-6 h-6" src="https://www.svgrepo.com/show/475656/google-color.svg" loading="lazy" alt="google logo">
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
