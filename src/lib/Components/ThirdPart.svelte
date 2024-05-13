<script>
	import Button from './Button.svelte';

	export let imageurl;
</script>

<div class=" flex flex-col mx-auto text-semibold text-slate-500 space-y-4">
	<img src={imageurl} alt="image" class="mx-auto" />
	<h1 class="mx-auto font-bold text-black">
		Drag and drop CAD models, assemblies or bulk import files.
	</h1>
	<p class="mx-auto">The files will only be processed locally and not stored on any server.</p>
	<p class=" mt-4 md:mx-[25%] mx-2 text-justify sm:text-center">
		Upload complex CAD models individually. You'll have the option to combine item details with
		identical names or SKUs from different files. For optimal merging of CAD and bulk import files,
		upload the CAD files before adding the bulk import files.
	</p>
	<h1 class="mx-auto my-2">OR</h1>
	<!-- <Button text={'Browse Files'} color={'bg-info'} type={'Button'} /> -->
</div>