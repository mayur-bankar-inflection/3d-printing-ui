<script lang="ts">
	import * as Table from '$lib/components/ui/table';
	import { AspectRatio } from '$lib/components/ui/aspect-ratio';
	import { Button } from '$lib/components/ui/button/index.js';

	const arrayOfObjects = [
		{
			key1: 'value1',
			key2: 'value2',
			key3: 'value3',
			key4: 'value4',
			key5: 'value5',
			key6: 'value6'
		},
		{
			key1: 'value1',
			key2: 'value2',
			key3: 'value3',
			key4: 'value4',
			key5: 'value5',
			key6: 'value6'
		},
		{
			key1: 'value1',
			key2: 'value2',
			key3: 'value3',
			key4: 'value4',
			key5: 'value5',
			key6: 'value6'
		},
		{
			key1: 'value1',
			key2: 'value2',
			key3: 'value3',
			key4: 'value4',
			key5: 'value5',
			key6: 'value6'
		},
		{
			key1: 'value1',
			key2: 'value2',
			key3: 'value3',
			key4: 'value4',
			key5: 'value5',
			key6: 'value6'
		},
		{
			key1: 'value1',
			key2: 'value2',
			key3: 'value3',
			key4: 'value4',
			key5: 'value5',
			key6: 'value6'
		}
	];
</script>

<div class="flex flex-wrap">
	<div class="w-full p-4 md:w-1/2 lg:w-1/2 xl:w-1/2">
		<div class="bg-gray-200">
			<Table.Root class="p-1">
				<Table.Header class="border-b-2 border-slate-400	">
					<Table.Row>
						<Table.Head>Sr No.</Table.Head>
						<Table.Head>Column</Table.Head>
						<Table.Head>Column</Table.Head>
						<Table.Head>Column</Table.Head>
						<Table.Head>Column</Table.Head>
						<Table.Head>Column</Table.Head>
						<Table.Head>Column</Table.Head>
						<Table.Head>Column</Table.Head>
					</Table.Row>
				</Table.Header>
				<Table.Body>
					{#each arrayOfObjects as a, index}
						<Table.Row class=" border-b border-slate-400">
							<Table.Cell class="font-medium">{index + 1}</Table.Cell>
							<Table.Cell>{a.key1}</Table.Cell>
							<Table.Cell>{a.key2}</Table.Cell>
							<Table.Cell class="text-left">{a.key3}</Table.Cell>
							<Table.Cell>{a.key4}</Table.Cell>
							<Table.Cell>{a.key5}</Table.Cell>
							<Table.Cell>{a.key6}</Table.Cell>
							<Table.Cell class="text-right">
								<Button variant="destructive">Button</Button>
							</Table.Cell>
						</Table.Row>
					{/each}
				</Table.Body>
				<Table.Caption>List of rows and columns.</Table.Caption>
			</Table.Root>
		</div>
	</div>
	<div class="w-full p-4 md:w-1/2 lg:w-1/2 xl:w-1/2">
		<div class="bg-gray-200 p-4">
			<AspectRatio ratio={16 / 9} class="bg-muted">
				<img src="..." alt="..." class="rounded-md object-cover" />
			</AspectRatio>
		</div>
	</div>
</div>
