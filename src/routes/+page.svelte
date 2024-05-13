<script>

	import FirstPart from "$lib/Components/FirstPart.svelte";
	import SecondPart from "$lib/Components/SecondPart.svelte";
	import ThirdPart from "$lib/Components/ThirdPart.svelte";
	import LastPart from "$lib/Components/LastPart.svelte";

</script>
<div class="bg-slate-200 h-fit w-full p-8 space-y-4">
	<FirstPart />
	<div class=" flex md:flex-row flex-col">
		<SecondPart
			imageurl={'import.png'}
			name={'Import'}
			description={'Start with CAD models or whole part inventories'}
			arrow={'arrow.png'}
		/>
		<SecondPart
			imageurl={'evaluate.png'}
			name={'Evaluate'}
			description={'Get AM estimates and manufacturability reports'}
			arrow={'arrow.png'}
		/>
		<SecondPart
			imageurl={'recycle.png'}
			name={'Refine'}
			description={'Find the best candidates and complete missing data'}
			arrow={'arrow.png'}
		/>
		<SecondPart
			imageurl={'order.png'}
			name={'Order'}
			description={'Order the parts from our service partners'}
			arrow={''}
		/>
	</div>

	<div class="h-fit w-full bg-white p-6 rounded-md shadow-md">
		<div class="border border-neutral-500 border-dashed h-full rounded-sm p-8">
			<ThirdPart imageurl={'upload.png'} />
		</div>
	</div>

	<div
		class="h-fit w-full p-4 flex bg-white flex-col sm:flex-row py-6 rounded-md shadow-md space-y-4"
	>
		<div class="flex flex-col">
			<h1 class="font-bold text-black text-xl">Still unsure?</h1>
			<p class="font-semibold text-md text-black">
				Test our web-app with demo data first. No commitment, just explore and see how it works!
			</p>
		</div>
		<div class="py-2 flex ">
			<!-- <Button text={'Try Demo'} color={'bg-white'} type={'input'} /> -->
			<input
				type="button"
				class="outline outline-info outline-2 mx-auto rounded-md text-info font-bold h-fit w-fit p-2 px-4 my-auto ml-[50%] justify-end items-end"
				name=""
				value="Try demo"
			/>
		</div>
	</div>

	<div class="h-fit w-full bg-slate-300 mx-auto py-10 px-12">
		<LastPart />
	</div>
</div>