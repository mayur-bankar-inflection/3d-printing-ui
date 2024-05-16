<script type="ts">
	import * as Card from '$lib/components/ui/card';
	import { Skeleton } from '$lib/components/ui/skeleton/index.ts';
</script>

<div class="mt-8 text-center text-2xl font-bold text-zinc-800 lg:mt-16 lg:text-3xl">
	ADDITIVE MANUFACTURING
</div>
<p class=" mx-auto mt-4 w-4/5 text-justify text-lg leading-loose text-gray-700 lg:mt-8 lg:text-xl">
	Incorporating additive manufacturing (AM) into your production process offers a transformative
	approach to manufacturing. Unlike traditional subtractive methods, which involve cutting away
	material to create a final product, AM builds objects layer by layer from digital designs. This
	innovative technique allows for greater design freedom, reduced waste, and the ability to create
	complex geometries that were previously impossible or impractical. By embracing AM, businesses can
	streamline prototyping, shorten lead times, and customize products to meet specific needs.
</p>

<!-- svelte-ignore a11y-distracting-elements -->
<div class="my-20 h-80 w-full bg-zinc-200 px-5 sm:h-fit">
	<p class="mx-auto mt-10 flex justify-center text-2xl font-bold text-zinc-800">COLLABORATIONS</p>
	<div class="hidden sm:flex">
		<marquee behavior="alternate" direction="left" scrollamount="10" scrolldelay="200" loop="3">
			<div class="m-4 flex flex-row p-4">
				<div class="m-4 bg-zinc-500 p-4">
					<div class="flex items-center space-x-4">
						<Skeleton class="h-12 w-12 rounded-full" />
						<div class="space-y-2">
							<Skeleton class="h-4 w-[250px]" />
							<Skeleton class="h-4 w-[250px]" />
						</div>
					</div>
				</div>
				<div class="m-4 bg-zinc-500 p-4">
					<div class="flex items-center space-x-4">
						<Skeleton class="h-12 w-12 rounded-full" />
						<div class="space-y-2">
							<Skeleton class="h-4 w-[250px]" />
							<Skeleton class="h-4 w-[200px]" />
						</div>
					</div>
				</div>
				<div class="m-4 bg-zinc-500 p-4">
					<div class="flex items-center space-x-4">
						<Skeleton class="h-12 w-12 rounded-full" />
						<div class="space-y-2">
							<Skeleton class="h-4 w-[250px]" />
							<Skeleton class="h-4 w-[250px]" />
						</div>
					</div>
				</div>
				<div class="m-4 bg-zinc-500 p-4">
					<div class="flex items-center space-x-4">
						<Skeleton class="h-12 w-12 rounded-full" />
						<div class="space-y-2">
							<Skeleton class="h-4 w-[250px]" />
							<Skeleton class="h-4 w-[200px]" />
						</div>
					</div>
				</div>
				<div class="m-4 bg-zinc-500 p-4">
					<div class="flex items-center space-x-4">
						<Skeleton class="h-12 w-12 rounded-full" />
						<div class="space-y-2">
							<Skeleton class="h-4 w-[250px]" />
							<Skeleton class="h-4 w-[250px]" />
						</div>
					</div>
				</div>
			</div>
		</marquee>
	</div>
	<div class="h-full p-2 sm:hidden">
		<marquee
			behavior="scroll"
			direction="up"
			scrollamount="10"
			scrolldelay="200"
			loop="3"
			height="250"
		>
			<div class="flex flex-col space-y-4">
				<div class=" bg-zinc-500 p-2">
					<div class="flex items-center space-x-4">
						<Skeleton class="h-12 w-12 rounded-full" />
						<div class="space-y-2">
							<Skeleton class="h-4 w-[200px]" />
							<Skeleton class="h-4 w-[150px]" />
						</div>
					</div>
				</div>
				<div class=" bg-zinc-500 p-2">
					<div class="flex items-center space-x-4">
						<Skeleton class="h-12 w-12 rounded-full" />
						<div class="space-y-2">
							<Skeleton class="h-4 w-[200px]" />
							<Skeleton class="h-4 w-[150px]" />
						</div>
					</div>
				</div>
				<div class=" bg-zinc-500 p-2">
					<div class="flex items-center space-x-4">
						<Skeleton class="h-12 w-12 rounded-full" />
						<div class="space-y-2">
							<Skeleton class="h-4 w-[200px]" />
							<Skeleton class="h-4 w-[150px]" />
						</div>
					</div>
				</div>
				<div class=" bg-zinc-500 p-2">
					<div class="flex items-center space-x-4">
						<Skeleton class="h-12 w-12 rounded-full" />
						<div class="space-y-2">
							<Skeleton class="h-4 w-[200px]" />
							<Skeleton class="h-4 w-[150px]" />
						</div>
					</div>
				</div>
			</div>
		</marquee>
	</div>
</div>

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

<!-- Highlights section -->
<div class="my-16">
	<div class="my-8 text-center text-2xl font-bold text-zinc-800 lg:mt-16 lg:text-3xl">
		HEIGHLIGHTS
	</div>

	<div class="mt-3 flex flex-wrap md:justify-center">
		<Card.Root
			class="bg-base-100 mb-3 mr-3 w-[390px] cursor-pointer rounded-xl  shadow-xl duration-300 hover:scale-95 "
		>
			<Card.Header>
				<figure class="  rounded-xl bg-zinc-800 p-10">
					<img src="/Dashboard/page.png" alt="page" class="mx-auto w-36" />
				</figure>
			</Card.Header>
			<Card.Content>
				<h2 class="card-title text-xl font-semibold text-orange-500">
					Single parts or bulk import
				</h2>
				<p class=" text-base">
					Upload CAD models of single parts and assemblies or import bulk data from your ERP system.
				</p>
			</Card.Content>
		</Card.Root>

		<Card.Root
			class="bg-base-100 mb-3 mr-3 w-[390px] cursor-pointer rounded-xl  shadow-xl duration-300 hover:scale-95 "
		>
			<Card.Header>
				<figure class=" rounded-xl bg-zinc-800 p-10">
					<img src="/Dashboard/refine1.png" alt="refine" class="mx-auto w-36" />
				</figure>
			</Card.Header>
			<Card.Content>
				<h2 class="card-title text-xl font-semibold text-orange-500">Comprehensive analysis</h2>
				<p class=" text-base">
					Quickly assess the suitability of your parts for AM. Identify the best AM process and
					material for your application and compare results to total cost of ownership calculations.
				</p>
			</Card.Content>
		</Card.Root>

		<Card.Root
			class="bg-base-100 mb-3 mr-3 w-[390px] cursor-pointer rounded-xl  shadow-xl duration-300 hover:scale-95 "
		>
			<Card.Header>
				<figure class=" rounded-xl bg-zinc-800 p-10">
					<img src="/Dashboard/lock.png" alt="lock" class="mx-auto w-36" />
				</figure>
			</Card.Header>
			<Card.Content>
				<h2 class="card-title text-xl font-semibold text-orange-500">Privacy by design</h2>
				<p class=" text-base">
					SelectAM is built as a hybrid web application. Your sensititve data is processed locally
					on your device and never leaves your network.
				</p>
			</Card.Content>
		</Card.Root>
	</div>
</div>
