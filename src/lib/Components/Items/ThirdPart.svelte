<script>
	import Button from '../ui/button/button.svelte';

	// import Button from './Button.svelte';

	export let imageurl;
</script>

<div class=" text-semibold mx-auto flex flex-col space-y-4 text-slate-500">
	<img src={imageurl} alt="image" class="mx-auto" />
	<h1 class="mx-auto font-bold text-black">
		Drag and drop CAD models, assemblies or bulk import files.
	</h1>
	<p class="mx-auto">The files will only be processed locally and not stored on any server.</p>
	<p class=" mx-2 mt-4 text-justify sm:text-center md:mx-[25%]">
		Lorem ipsum, dolor sit amet consectetur adipisicing elit. Culpa nam sed voluptatum magnam iure,
		voluptatibus veritatis voluptas odit doloribus eveniet, impedit a eius mollitia neque, dolor at?
		Unde, repudiandae fugit?
	</p>
	<h1 class="mx-auto my-2">OR</h1>
	<!-- <Button text={'Browse Files'} color={'bg-info'} type={'Button'} /> -->
	<Button class="mx-auto px-12 sm:w-fit">Button</Button>
</div>
