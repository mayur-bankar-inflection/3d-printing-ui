<script>
	import Button from '../ui/button/button.svelte';

	// import Button from './Button.svelte';

	export let imageurl;
</script>

<div class="space-y-4 text-center text-slate-500">
	<img src={imageurl} alt="image" class="mx-auto" />
	<h1 class="font-bold text-black">Drag and drop CAD models, assemblies, or bulk import files.</h1>
	<p>The files will only be processed locally and not stored on any server.</p>
	<p
		class="mx-auto mt-4 text-justify sm:text-center md:max-w-md lg:max-w-lg xl:max-w-xl 2xl:max-w-2xl"
	>
		Lorem ipsum, dolor sit amet consectetur adipisicing elit. Culpa nam sed voluptatum magnam iure,
		voluptatibus veritatis voluptas odit doloribus eveniet, impedit a eius mollitia neque, dolor at?
		Unde, repudiandae fugit?
	</p>
	<h1 class="my-2">OR</h1>
	<Button class="mx-auto px-12 sm:w-fit">Button</Button>
</div>
