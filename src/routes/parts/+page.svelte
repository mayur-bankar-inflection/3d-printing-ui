<script>
	import { Button } from '$lib/Components/ui/button';
</script>

<div class="mt-8 text-center text-2xl font-bold text-zinc-800 lg:mt-16 lg:text-3xl">
	IMPORT DATA
</div>
<p class=" mx-auto mt-4 w-4/5 text-justify text-lg leading-loose text-gray-700 lg:mt-8 lg:text-xl">
	Choose the files you want to add. Keep in mind that the time it takes to process these files can
	change based on their size and your computer's processing capabilities. Once the files are
	imported, you'll receive estimated values for the items, identify the best prospects for Additive
	Manufacturing (AM), and have the option to order them through our service partner.
</p>

<div class="mx-auto mt-6 flex w-4/5 flex-col py-4 lg:flex-row lg:items-center">
	<div class="flex items-center">
		<p class="h-20 rounded-full bg-zinc-800">
			<img src="/Dashboard/import.png" alt="" class="h-20 w-20 p-4" />
		</p>

		<div class="ml-3 w-2/3">
			<h1 class=" text-xl font-semibold text-orange-500">Import</h1>
			<p class=" text-gray-600">Start with CAD models or whole part inventories</p>
		</div>
	</div>

	<div class="lg:m-2">
		<img src="/Dashboard/arrow.png" class=" rotate-90 lg:rotate-0" alt="" />
	</div>

	<div class="flex items-center">
		<p class="h-20 rounded-full bg-zinc-800">
			<img src="/Dashboard/evaluate.png" alt="" class="w-20 p-3" />
		</p>

		<div class="ml-3 w-2/3">
			<h1 class=" text-xl font-semibold text-orange-500">Evaluate</h1>
			<p class=" text-gray-600">Get AM estimates and manufacturability reports</p>
		</div>
	</div>

	<div class="lg:m-2">
		<img src="/Dashboard/arrow.png" class=" rotate-90 lg:rotate-0" alt="" />
	</div>

	<div class="flex items-center">
		<div class="h-20 rounded-full bg-zinc-800">
			<img src="/Dashboard/refine.png" alt="" class="w-20 p-3" />
		</div>

		<div class="ml-3 w-3/4">
			<h1 class=" text-xl font-semibold text-orange-500">Refine</h1>
			<p class=" text-gray-600">Find the best candidates and complete missing data</p>
		</div>
	</div>

	<div class="lg:m-2">
		<img src="/Dashboard/arrow.png" class=" rotate-90 lg:rotate-0" alt="" />
	</div>

	<div class="flex items-center">
		<p class="h-20 rounded-full bg-zinc-800">
			<img src="/Dashboard/order.png" alt="" class="w-20 p-4" />
		</p>

		<div class="ml-3 w-2/3">
			<h1 class=" text-xl font-semibold text-orange-500">Order</h1>
			<p class=" text-gray-600">Order the parts from our service partners</p>
		</div>
	</div>
</div>

<div class="w-full rounded-md bg-white p-6 shadow-md">
	<div class="border border-dashed border-neutral-500 p-8 w-4/5 mx-auto">
		<div class="space-y-4 text-center text-slate-500">
			<img src="/Estimation/importblack.png" alt="image" class="mx-auto " />
			<h1 class="font-bold text-zinc-800 text-xl">
				Drag and drop CAD models, assemblies, or bulk import files.
			</h1>
			<p>The files will only be processed locally and not stored on any server.</p>
			<p
				class="mx-auto mt-4 text-justify sm:text-center md:max-w-md lg:max-w-lg xl:max-w-xl 2xl:max-w-2xl"
			>
				Lorem ipsum, dolor sit amet consectetur adipisicing elit. Culpa nam sed voluptatum magnam
				iure, voluptatibus veritatis voluptas odit doloribus eveniet, impedit a eius mollitia neque,
				dolor at? Unde, repudiandae fugit?
			</p>
			<h1 class="my-2">OR</h1>
			<Button class="mx-auto px-12 sm:w-fit">Browse Files</Button>
		</div>
	</div>
</div>
