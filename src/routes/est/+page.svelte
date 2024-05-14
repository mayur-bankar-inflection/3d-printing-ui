<script lang="ts">
	import * as Select from '$lib/components/ui/select/index.js';
	import { Button } from '$lib/components/ui/button/index.js';

	const technology = [
		{ value: 'apple', label: 'Sintering' },
		{ value: 'banana', label: 'Melting' },
		{ value: 'blueberry', label: 'Sintering' },
		{ value: 'grapes', label: 'Melting' },
		{ value: 'grapes', label: 'Melting' },
		{ value: 'pineapple', label: 'Sintering' }
	];

	const country = [
		{ value: 'India', label: 'India' },
		{ value: 'United States', label: 'United States' },
		{ value: 'Canada', label: 'Canada' },
		{ value: 'Brazil', label: 'Brazil' },
		{ value: 'United Kingdom', label: 'United Kingdom' },
		{ value: 'France', label: 'France' },
		{ value: 'Germany', label: 'Germany' },
		{ value: 'Italy', label: 'Italy' },
		{ value: 'Spain', label: 'Spain' },
		{ value: 'Australia', label: 'Australia' },
		{ value: 'China', label: 'China' },
		{ value: 'Japan', label: 'Japan' },
		{ value: 'South Korea', label: 'South Korea' },
		{ value: 'Russia', label: 'Russia' }
	];

	let count = 0;
	const increment = () => {
		if (count == 10) {
			return;
		} else {
			count += 1;
		}
	};
	const decrement = () => {
		if (count == 0) {
			return;
		} else {
			count -= 1;
		}
	};
</script>

<div class="mx-auto my-5 w-3/4">
	<!-- <div class="flex flex-row">
		<div>
			<p class="text-xl font-bold">(Online Calculator)</p>
			<p>1 model (1configuration)</p>
		</div>
		<div class="float-right my-auto items-end justify-end">
			<Button variant="outline">Outline</Button>
			<Button variant="outline">Outline</Button>
		</div>
	</div> -->
	<div class="flex flex-col">
		<div class="flex-grow">
			<p class="text-xl font-bold">(Online Calculator)</p>
			<p>1 model (1configuration)</p>
		</div>
		<div class="flex justify-end space-x-4">
			<Button variant="outline" class="rounded-sm border-4 border-cyan-400 bg-white px-8 py-1"
				>Support</Button
			>
			<Button variant="outline" class="rounded-sm border-4 border-cyan-400 bg-white px-8 py-1"
				>Options</Button
			>
		</div>
	</div>
	<!-- <div class="flex flex-col ">
        <div class="flex-grow">
            <p class="text-xl font-bold">(Online Calculator)</p>
            <p>1 model (1 configuration)</p>
        </div>
        <div class="flex justify-end  space-x-4">
            <button class="bg-white border border-gray-400 px-4 py-2 rounded-lg">Outline</button>
            <button class="bg-white border border-gray-400 px-4 py-2 rounded-lg">Outline</button>
        </div>
    </div> -->
	<div class="mt-5 rounded-lg border border-black">
		<div class="border border-black p-4 py-6 font-bold">Configuration 1, 1 model</div>
		<div class="flex flex-row space-x-4 p-4">
			<div class="w-2/4 space-y-4">
				<div class="flex h-fit w-full flex-row space-x-10 rounded-md bg-slate-200 p-4 pb-1">
					<div class=" w-fit">
						<img src="Items/arrow.png" alt="" class="w-32" />
						<p>All images</p>
					</div>
					<div class=" w-full p-3 pb-1">
						<p class="font-bold">Name</p>
						<p>Diamensions</p>
						<div class="flex w-full flex-row space-x-5">
							<div>
								<div class="mt-5 flex items-center justify-center">
									<button
										class="rounded-l bg-slate-300 px-4 py-2 font-bold text-black hover:bg-slate-400"
										on:click={decrement}
									>
										-
									</button>
									<span class="bg-gray-200 px-4 py-2">{count}</span>
									<button
										class="rounded-r bg-slate-300 px-4 py-2 font-bold text-black hover:bg-slate-400"
										on:click={increment}
									>
										+
									</button>
								</div>
							</div>
							<div class="mt-1 w-full items-end justify-end pt-2">
								<p class="text-end">Pricing</p>
								<p class="text-end">EUR 48.32</p>
								<p class="text-end font-bold">EUR 123.20</p>
							</div>
						</div>
					</div>
				</div>
				<div
					class="h-fit w-full space-y-5 rounded-md border-2 border-dashed border-slate-400 bg-slate-200 p-4"
				>
					<div class="flex flex-row space-x-20">
						<Button variant="ghost">Drag file here</Button>
						<p class="mx-auto mt-2 flex justify-center">OR</p>
						<Button variant="outline" class="outline-blue-400">Select files</Button>
					</div>
					<p class="mx-auto flex justify-center">Extensions allowed</p>
				</div>
			</div>
			<div class="mx-auto w-2/4 space-y-4">
				<div class=" ">
					<Select.Root portal={null}>
						<Select.Trigger class="w-full">
							<Select.Value placeholder="Select a Technology" />
						</Select.Trigger>
						<Select.Content>
							<Select.Group>
								<Select.Label>Technology</Select.Label>
								{#each technology as technology}
									<Select.Item value={technology.value} label={technology.label}
										>{technology.label}</Select.Item
									>
								{/each}
							</Select.Group>
						</Select.Content>
						<Select.Input name="favoritetechnology" />
					</Select.Root>
				</div>
				<div class="">
					<Select.Root portal={null}>
						<Select.Trigger class="w-full">
							<Select.Value placeholder="Material" />
						</Select.Trigger>
						<Select.Content>
							<Select.Group>
								<Select.Label>Technology</Select.Label>
								{#each technology as technology}
									<Select.Item value={technology.value} label={technology.label}
										>{technology.label}</Select.Item
									>
								{/each}
							</Select.Group>
						</Select.Content>
						<Select.Input name="favoritetechnology" />
					</Select.Root>
				</div>
				<div class="">
					<Select.Root portal={null}>
						<Select.Trigger class="w-full">
							<Select.Value placeholder="Post Processing" />
						</Select.Trigger>
						<Select.Content>
							<Select.Group>
								<Select.Label>Technology</Select.Label>
								{#each technology as technology}
									<Select.Item value={technology.value} label={technology.label}
										>{technology.label}</Select.Item
									>
								{/each}
							</Select.Group>
						</Select.Content>
						<Select.Input name="favoritetechnology" />
					</Select.Root>
				</div>
				<Button class="mx-auto flex w-10/12">Material wizard</Button>
			</div>
		</div>
	</div>
</div>
<div class="mx-auto my-auto flex h-fit w-full flex-row bg-slate-400 px-4 py-10">
	<div class="mx-auto flex w-6/12 justify-end">
		<p class="font-bold">Your estimatimate price incl. shipping: EUR 132.20</p>
		<Button variant="outline" class="ml-5 rounded-sm border px-8 py-1 text-cyan-600"
			>Price Details and Options</Button
		>
	</div>
	<div class="ml-1 w-6/12 pl-32">
		<Select.Root portal={null}>
			<Select.Trigger class="w-3/5">
				<Select.Value placeholder="Delivery Country" />
			</Select.Trigger>
			<Select.Content>
				<Select.Group>
					<Select.Label>Country</Select.Label>
					{#each country as country}
						<Select.Item value={country.value} label={country.label}>{country.label}</Select.Item>
					{/each}
				</Select.Group>
			</Select.Content>
			<Select.Input name="favoritecountry" />
		</Select.Root>
	</div>
</div>
