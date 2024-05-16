<script type="ts">
	import { Button } from '$lib/Components/ui/button';
	import * as Card from '$lib/components/ui/card';
	import * as Table from '$lib/components/ui/table';
	// import { AspectRatio } from '$lib/components/ui/aspect-ratio';
	const arrayOfObjects = [
		{
			key1: 'Super Gear',
			key2: 'Nylon PA',
			key3: '...',
			key4: '$86.32',
			key5: '-86.32'
		},
		{
			key1: 'Super Gear',
			key2: 'Nylon PA',
			key3: '...',
			key4: '$86.32',
			key5: '-86.32'
		},
		{
			key1: 'Super Gear',
			key2: 'Nylon PA',
			key3: '...',
			key4: '$86.32',
			key5: '-86.32'
		},
		{
			key1: 'Super Gear',
			key2: 'Nylon PA',
			key3: '...',
			key4: '$86.32',
			key5: '-86.32'
		}
	];
</script>

<div class="my-8 text-center text-xl font-bold text-zinc-800 lg:mt-16 lg:text-2xl">DASHBOARD</div>
<div class="mt-3 flex flex-wrap justify-center">
	<Card.Root class="  m-4 flex w-[450px] shadow-xl ">
		<figure class=" rounded-sm p-3">
			<img src="Estimation/savings.png" alt="page" class="mx-auto w-16" />
		</figure>
		<Card.Content>
			<h1 class="card-title my-1 text-xl font-semibold text-yellow-500">AM Saving Potential</h1>
			<p>Total potential saving through AM</p>
			<h2 class="text-2xl font-bold">40,000</h2>
			<p>6 years 76 days average parts lifecycle</p>
		</Card.Content>
	</Card.Root>
	<Card.Root class="  m-4 flex w-[450px] shadow-xl ">
		<figure class=" rounded-sm p-3">
			<img src="Estimation/chart.png" alt="page" class="mx-auto w-14" />
		</figure>
		<Card.Content>
			<h1 class="card-title my-1 text-xl font-semibold text-yellow-500">AM Buisness Cases</h1>
			<p>High criteria score</p>
			<h2 class="text-2xl font-bold">81</h2>
			<p>29.51%</p>
		</Card.Content>
	</Card.Root>
	<Card.Root class=" m-4 flex w-[450px] shadow-xl ">
		<figure class=" rounded-sm p-3">
			<img src="Estimation/certify.png" alt="page" class="mx-auto w-16" />
		</figure>
		<Card.Content>
			<h1 class="card-title my-1 text-xl font-semibold text-yellow-500">AM Score</h1>
			<p>Score average</p>
			<h2 class="text-2xl font-bold">65.67/100</h2>
			<p>6 years 76 days average parts lifecycle</p>
		</Card.Content>
	</Card.Root>
	<Card.Root class=" m-4  flex w-[450px] shadow-xl ">
		<figure class=" rounded-sm p-3">
			<img src="Estimation/time.png" alt="page" class="mx-auto w-14" />
		</figure>
		<Card.Content>
			<h1 class="card-title my-1 text-xl font-semibold text-yellow-500">Shorter Lead Time</h1>
			<p>Decreased lead time</p>
			<h2 class="text-2xl font-bold">225</h2>
			<p>85.12%</p>
		</Card.Content>
	</Card.Root>
	<Card.Root class=" m-4 flex w-[450px] shadow-xl ">
		<figure class=" rounded-sm p-3">
			<img src="Estimation/quality.png" alt="page" class="mx-auto w-16" />
		</figure>
		<Card.Content>
			<h1 class="card-title my-1 text-xl font-semibold text-yellow-500">Data Quality</h1>
			<p>Validity of import data</p>
			<h2 class="text-2xl font-bold">86.25%</h2>
			<p>Data need to be checked</p>
		</Card.Content>
	</Card.Root>
	<Card.Root class=" m-4 flex w-[450px] shadow-xl ">
		<figure class=" rounded-sm p-3">
			<img src="Estimation/all.png" alt="page" class="mx-auto w-16" />
		</figure>
		<Card.Content>
			<h1 class="card-title my-1 text-xl font-semibold text-yellow-500">All Parts</h1>
			<p>Parts from models or import files</p>
			<h2 class="text-2xl font-bold">311</h2>
			<p>12 files have been imported</p>
		</Card.Content>
	</Card.Root>
</div>
<div class="mx-4 my-8 overflow-hidden rounded-lg shadow-lg md:mx-12">
	<div class="flex flex-wrap">
		<div class="w-full">
			<div class="">
				<Table.Root class="">
					<Table.Header class="border-b-2  bg-gray-200 text-base font-semibold    ">
						<Table.Row>
							<Table.Head>Name</Table.Head>
							<Table.Head>AM Material</Table.Head>
							<Table.Head>Model</Table.Head>
							<Table.Head>Average Price</Table.Head>
							<Table.Head>Savings</Table.Head>
							<Table.Head></Table.Head>
						</Table.Row>
					</Table.Header>
					<Table.Body>
						{#each arrayOfObjects as a, index}
							<Table.Row class=" border-b text-base ">
								<Table.Cell>{a.key1}</Table.Cell>
								<Table.Cell>{a.key2}</Table.Cell>
								<Table.Cell class="">{a.key3}</Table.Cell>
								<Table.Cell>{a.key4}</Table.Cell>
								<Table.Cell>{a.key5}</Table.Cell>
								<Table.Cell class="text-center">
									<Button>Button</Button>
								</Table.Cell>
							</Table.Row>
						{/each}
					</Table.Body>
				</Table.Root>
			</div>
		</div>
	</div>
</div>
