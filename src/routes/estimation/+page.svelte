<script lang="ts">
	import * as Select from '$lib/components/ui/select/index.js';
	import { Button } from '$lib/Components/ui/button';

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
	<div class="flex w-full flex-col items-center md:flex-row">
		<div class="flex-grow text-center md:text-start">
			<p class="text-xl font-bold">(Online Calculator)</p>
			<p>1 model (1configuration)</p>
		</div>
		<div class="my-6 flex justify-end space-x-6">
			<Button>Support</Button>
			<Button>Options</Button>
		</div>
	</div>

	<div class="mt-5 w-full rounded-lg border-2 border-black">
		<div class="border-b-2 border-black p-4 py-6 font-bold">Configuration 1, 1 model</div>
		<div class="flex flex-col space-x-0 space-y-2 p-4 sm:flex-row sm:space-x-2">
			<div class="flex w-full flex-col space-y-4 sm:w-2/4">
				<div
					class="flex h-fit w-full flex-col rounded-md bg-slate-100 p-4 pb-1 sm:flex-row sm:space-x-10"
				>
					<div class=" w-full sm:w-fit">
						<img src="Estimation/part.png" alt="" class="w-full sm:w-32" />
					</div>
					<div class=" w-full p-3 pb-1 sm:w-fit">
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
					class="h-fit w-full space-y-5 rounded-md border border-dashed border-zinc-800 bg-slate-100 p-4"
				>
					<div class="lg:sapce-x-20 flex flex-col sm:flex-row sm:space-x-5 md:space-x-10">
						<Button variant="ghost">Drag file here</Button>
						<p class="mx-auto mt-2 flex justify-center">OR</p>
						<Button variant="outline" class="outline-blue-400">Select files</Button>
					</div>
					<p class="mx-auto flex justify-center">Extensions allowed</p>
				</div>
			</div>
			<div class="w-full space-y-4 p-2 sm:w-2/4">
				<div class=" mt-2">
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
				<Button class="mx-auto flex w-full ">Material wizard</Button>
			</div>
		</div>
	</div>
</div>

<div class="my-6 flex flex-wrap items-center justify-center">
	<p class="p-4 text-lg font-semibold">Your price incl.shipping: EUR 152.15</p>
	<Button class="mx-4 my-4 border-2 hover:text-white">Price Details and Options</Button>
	<Select.Root portal={null}>
		<Select.Trigger class="ml-4 w-56">
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
