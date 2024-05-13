<script type="ts">
	import * as Card from '$lib/components/ui/card';
	import { Button } from '$lib/components/ui/button/index';
</script>

<div class="px-7 py-5">
	<div class=" bg-gradient-to-br from-green-600 to-zinc-400 p-8 rounded-lg">
		<div class=" md:ml-8">
			<h1 class=" text-3xl md:text-4xl lg:text-5xl text-white font-semibold">
				Optimize manufacturing workflows.
			</h1>
			<p class="text-xl md:text-2xl lg:text-3xl mt-3 text-slate-50">
				Maximize the benefits of additive manufacturing for your business.
				<br /> <span>Discover. Evaluate. Purchase.</span>
			</p>

			<Button
				variant="outline"
				class="bg-transparent text-white hover:bg-slate-200 hover:text-black duration-300 mt-3"
				>Get Started</Button
			>
		</div>
	</div>

	<div class=" m-10 text-center flex justify-center">
		<div class="w-2/3">
			<p>Service Offerings and Available Resources</p>
			<h1 class=" text-3xl font-bold">Enhance Your Perspective</h1>
			<p class=" text-lg mt-4">
				Explore the next frontier in additive manufacturing (AM) evaluation through our cutting-edge
				solution. Analyze AM market rates, juxtapose them with traditional manufacturing expenses,
				and evaluate manufacturability securely, without the need to upload CAD models to a server,
				safeguarding your data privacy. Transform your manufacturing approach today.
			</p>
		</div>
	</div>

	<div class="mt-6 flex flex-col lg:flex-row lg:items-center">
		<div class="flex items-center">
			<p class="bg-gradient-to-br from-teal-500 to-zinc-400 rounded-full h-20">
				<img src="import.png" alt="" class="p-4 w-20" />
			</p>

			<div class="ml-3 w-2/3">
				<h1 class=" font-semibold text-lg">Import</h1>
				<p class=" text-gray-600">Start with CAD models or whole part inventories</p>
			</div>
		</div>

		<div class="lg:m-2">
			<img src="arrow-r.png" class=" rotate-90 lg:rotate-0" alt="" />
		</div>

		<div class="flex items-center">
			<p class="bg-gradient-to-br from-teal-500 to-zinc-400 rounded-full h-20">
				<img src="evaluate.png" alt="" class="p-3 w-20" />
			</p>

			<div class="ml-3 w-2/3">
				<h1 class=" font-semibold text-lg">Evaluate</h1>
				<p class=" text-gray-600">Get AM estimates and manufacturability reports</p>
			</div>
		</div>

		<div class="lg:m-2">
			<img src="arrow-r.png" class=" rotate-90 lg:rotate-0" alt="" />
		</div>

		<div class="flex items-center">
			<div class="bg-gradient-to-br from-teal-500 to-zinc-400 rounded-full h-20">
				<img src="import.png" alt="" class="p-3 w-20" />
			</div>

			<div class="ml-3 w-3/4">
				<h1 class=" font-semibold text-lg">Refine</h1>
				<p class=" text-gray-600">Find the best candidates and complete missing data</p>
			</div>
		</div>

		<div class="lg:m-2">
			<img src="arrow-r.png" class=" rotate-90 lg:rotate-0" alt="" />
		</div>

		<div class="flex items-center">
			<p class="bg-gradient-to-br from-teal-500 to-zinc-400 rounded-full h-20">
				<img src="order.png" alt="" class="w-20 p-4" />
			</p>

			<div class="ml-3 w-2/3">
				<h1 class=" font-semibold text-lg">Order</h1>
				<p class=" text-gray-600">Order the parts from our service partners</p>
			</div>
		</div>
	</div>

	<!-- Highlights section -->
	<div class="mt-16">
		<h1 class=" font-bold text-3xl">Highlights</h1>

		<div class="mt-3 flex flex-wrap md:justify-center">
			<Card.Root
				class="w-[390px] bg-base-100 shadow-xl mr-3 mb-3 hover:border-teal-500 cursor-pointer hover:scale-95 duration-300"
			>
				<Card.Header>
					<figure class=" bg-blue-400 p-3 rounded-sm">
						<img src="page1.png" alt="page" class="w-40" />
					</figure>
				</Card.Header>
				<Card.Content>
					<h2 class="card-title font-bold">Single parts or bulk import</h2>
					<p class=" text-base">
						Upload CAD models of single parts and assemblies or import bulk data from your ERP
						system.
					</p>
				</Card.Content>
			</Card.Root>

			<Card.Root
				class="w-[390px] bg-base-100 shadow-xl mr-3 mb-3  hover:border-teal-500 cursor-pointer hover:scale-95 duration-300"
			>
				<Card.Header>
					<figure class=" bg-rose-400">
						<img src="import1.png" alt="import" class="w-40" />
					</figure>
				</Card.Header>
				<Card.Content>
					<h2 class="card-title font-bold">Comprehensive analysis</h2>
					<p class=" text-base">
						Quickly assess the suitability of your parts for AM. Identify the best AM process and
						material for your application and compare results to total cost of ownership
						calculations.
					</p>
				</Card.Content>
			</Card.Root>

			<Card.Root
				class="w-[390px] bg-base-100 shadow-xl mr-3 mb-3  hover:border-teal-500 cursor-pointer hover:scale-95 duration-300"
			>
				<Card.Header>
					<figure class=" bg-emerald-600 p-3">
						<img src="lock.png" alt="lock" class="w-40" />
					</figure>
				</Card.Header>
				<Card.Content>
					<h2 class="card-title font-bold">Privacy by design</h2>
					<p class=" text-base">
						SelectAM is built as a hybrid web application. Your sensititve data is processed locally
						on your device and never leaves your network.
					</p>
				</Card.Content>
			</Card.Root>
		</div>
	</div>

	<div class=" flex justify-center items-center mt-20">
		<img src="AM.jpg" alt="" class="rounded-md shadow-md" />
		<div class=" drop-shadow-xl ml-6 w-96 text-xl">
			<p>
				We aim to democratize the advanced manufacturing of metallic components, striving to make it
				accessible, straightforward, and sustainable. Our goal is to foster an innovative and
				environmentally conscious manufacturing sector that serves our customers both in the UK and
				around the globe.
			</p>
		</div>
	</div>

	<div class="flex justify-center ">
	<Card.Root
		class="hover:scale-105 duration-200 bg-base-100 shadow-xl mr-3 mb-3 hover:border-teal-500 cursor-pointer flex justify-center flex-col items-center w-[600px] mt-10 bg-slate-700 bg-opacity-25"
	>
		<Card.Header>
			<h1 class="font-semibold text-2xl mb-3">Get in touch</h1>
		</Card.Header>
		<Card.Content>
			<div>
				<input type="text" placeholder="Name" class="mb-2 p-2 rounded-sm outline-none" />
				<input type="text" placeholder="Email" class="p-2 rounded-sm outline-none" />
			</div>
			<div class="flex flex-col">
				<input type="text" placeholder="Subject" class="mb-4 p-2 rounded-sm outline-none" />
				<textarea rows="5" cols="6" placeholder="Message" id="" class="p-2 outline-none rounded-sm"
				></textarea>
			</div>

			<Button
				variant="outline"
				class="bg-green-600 text-white hover:bg-green-700 hover:text-white duration-300 mt-3"
				>Send Message</Button
			>
		</Card.Content>
	</Card.Root>
</div>
</div>
