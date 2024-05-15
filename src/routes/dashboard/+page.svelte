<script type="ts">
	import { Button } from '$lib/Components/ui/button';
	import * as Card from '$lib/Components/ui/card';
</script>

<div class="my-8 text-center text-xl font-bold text-zinc-800 lg:mt-16 lg:text-2xl">DASHBOARD</div>

<div class="mt-3 flex flex-wrap justify-center">
	<Card.Root class="  m-4 flex w-[450px] shadow-xl ">
		<figure class=" rounded-sm p-3">
			<img src="Estimation/savings.png" alt="page" class="mx-auto w-16" />
		</figure>
		<Card.Content>
			<h1 class="card-title my-1 text-xl font-semibold text-orange-500">AM Saving Potential</h1>
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
			<h1 class="card-title my-1 text-xl font-semibold text-orange-500">AM Buisness Cases</h1>
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
			<h1 class="card-title my-1 text-xl font-semibold text-orange-500">AM Score</h1>
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
			<h1 class="card-title my-1 text-xl font-semibold text-orange-500">Shorter Lead Time</h1>
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
			<h1 class="card-title my-1 text-xl font-semibold text-orange-500">Data Quality</h1>
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
			<h1 class="card-title my-1 text-xl font-semibold text-orange-500">All Parts</h1>
			<p>Parts from models or import files</p>
			<h2 class="text-2xl font-bold">311</h2>
			<p>12 files have been imported</p>
		</Card.Content>
	</Card.Root>
</div>

<div class="mx-4 my-8 overflow-hidden rounded-lg shadow-lg md:mx-12">
	<table class="w-full table-fixed">
		<thead>
			<tr class="bg-zinc-800">
				<th class="w-1/4 px-6 py-4 text-left font-semibold uppercase text-white">Name</th>
				<th class="w-1/4 px-6 py-4 text-left font-semibold uppercase text-white">AM Material</th>
				<th class="w-1/4 px-6 py-4 text-left font-semibold uppercase text-white">Model</th>
				<th class="w-1/4 px-6 py-4 text-left font-semibold uppercase text-white">Average Price</th>
				<th class="w-1/4 px-6 py-4 text-left font-semibold uppercase text-white">Savings</th>
				<th class="w-1/4 px-6 py-4 text-left font-semibold uppercase text-white"></th>
			</tr>
		</thead>
		<tbody class="bg-white">
			<tr>
				<td class="border-b border-gray-200 px-6 py-4">Spur Gear</td>
				<td class="truncate border-b border-gray-200 px-6 py-4">Nylon PA</td>
				<td class="border-b border-gray-200 px-6 py-4">...</td>
				<td class="border-b border-gray-200 px-6 py-4">$86.22</td>
				<td class="border-b border-gray-200 px-6 py-4">-86.22</td>
				<td class="border-b border-gray-200 px-6 py-4"><Button>Order</Button></td>
			</tr>
			<tr>
				<td class="border-b border-gray-200 px-6 py-4">Spur Gear</td>
				<td class="truncate border-b border-gray-200 px-6 py-4">Nylon PA</td>
				<td class="border-b border-gray-200 px-6 py-4">...</td>
				<td class="border-b border-gray-200 px-6 py-4">$66.22</td>
				<td class="border-b border-gray-200 px-6 py-4">+86.22</td>
				<td class="border-b border-gray-200 px-6 py-4"><Button>Order</Button></td>
			</tr>
			<tr>
				<td class="border-b border-gray-200 px-6 py-4">Spur Gear</td>
				<td class="truncate border-b border-gray-200 px-6 py-4">Nylon PA</td>
				<td class="border-b border-gray-200 px-6 py-4">...</td>
				<td class="border-b border-gray-200 px-6 py-4">$54.22</td>
				<td class="border-b border-gray-200 px-6 py-4">-86.22</td>

				<td class="border-b border-gray-200 px-6 py-4"><Button>Order</Button></td>
			</tr>
			<tr>
				<td class="border-b border-gray-200 px-6 py-4">Spur Gear</td>
				<td class="truncate border-b border-gray-200 px-6 py-4">Nylon PA</td>
				<td class="border-b border-gray-200 px-6 py-4">...</td>
				<td class="border-b border-gray-200 px-6 py-4">$72.22</td>
				<td class="border-b border-gray-200 px-6 py-4">+86.22</td>

				<td class="border-b border-gray-200 px-6 py-4"><Button>Order</Button></td>
			</tr>
		</tbody>
	</table>
</div>
