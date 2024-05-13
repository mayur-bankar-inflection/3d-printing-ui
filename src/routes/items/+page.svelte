<script>
	import FirstPart from '$lib/Components/Items/FirstPart.svelte';
	import SecondPart from '$lib/Components/Items/SecondPart.svelte';
	import ThirdPart from '$lib/Components/Items/ThirdPart.svelte';
	import LastPart from '$lib/Components/Items/LastPart.svelte';
	import Cards from '$lib/Components/Items/Cards.svelte';
</script>

<div class="h-fit w-full space-y-4 bg-slate-200 p-8">
	<FirstPart />
	<div class=" flex flex-col md:flex-row">
		<SecondPart
			imageurl={'Items/import.png'}
			name={'Import'}
			description={'Start with CAD models or whole part inventories'}
			arrow={'arrow.png'}
		/>
		<SecondPart
			imageurl={'Items/evaluate.png'}
			name={'Evaluate'}
			description={'Get AM estimates and manufacturability reports'}
			arrow={'arrow.png'}
		/>
		<SecondPart
			imageurl={'Items/recycle.png'}
			name={'Refine'}
			description={'Find the best candidates and complete missing data'}
			arrow={'arrow.png'}
		/>
		<SecondPart
			imageurl={'Items/order.png'}
			name={'Order'}
			description={'Order the parts from our service partners'}
			arrow={''}
		/>
	</div>

	<div class="h-fit w-full rounded-md bg-white p-6 shadow-md">
		<div class="h-full rounded-sm border border-dashed border-neutral-500 p-8">
			<ThirdPart imageurl={'Items/upload.png'} />
		</div>
	</div>

	<!-- <div
					class="flex h-fit w-full flex-col space-y-4 rounded-md bg-white p-4 py-6 shadow-md sm:flex-row"
				>
					<div class="flex flex-col">
						<h1 class="text-xl font-bold text-black">Still unsure?</h1>
						<p class="text-md font-semibold text-black">
							Test our web-app with demo data first. No commitment, just explore and see how it works!
						</p>
					</div>
					<div class="flex py-2">
						<input
							type="button"
							class="mx-auto my-auto ml-[50%] h-fit w-fit items-end justify-end rounded-md p-2 px-4 font-bold text-cyan-500 outline outline-2 outline-cyan-500"
							name=""
							value="Try demo"
						/>
					</div>
				</div> -->

	<div
		class="flex h-fit w-full flex-col space-y-2 rounded-md shadow-md sm:flex-col sm:p-4 sm:py-6 lg:flex-row"
	>
		<Cards />
		<Cards />
		<Cards />
		<Cards />
	</div>

	<div class="mx-auto h-fit w-full bg-slate-300 px-12 py-10">
		<LastPart />
	</div>
</div>
