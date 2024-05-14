<script lang="ts">
	import * as Table from '$lib/components/ui/table';
	import { AspectRatio } from '$lib/components/ui/aspect-ratio';
	import { Button } from "$lib/components/ui/button/index.js";
</script>

<div class="flex flex-wrap">
	<div class="w-full p-4 md:w-1/2 lg:w-1/2 xl:w-1/2">
		<div class="bg-gray-200 ">
			<Table.Root class="p-1">
				<Table.Header class="border-slate-400 border-b-2	">
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
					<Table.Row class=" border-slate-400 border-b">
						<Table.Cell class="font-medium">1</Table.Cell>
						<Table.Cell>Row 1</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell class="text-left">cell</Table.Cell>
						<Table.Cell> cell</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell class="text-right">
							<Button variant="destructive">Button</Button>
						</Table.Cell>
					</Table.Row>
					<Table.Row class=" border-slate-400 border-b">
						<Table.Cell class="font-medium">2</Table.Cell>
						<Table.Cell>Row 1</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell class="text-left">cell</Table.Cell>
						<Table.Cell> cell</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell class="text-right">
							<Button variant="destructive">Button</Button>
						</Table.Cell>
					</Table.Row>
					<Table.Row class=" border-slate-400 border-b">
						<Table.Cell class="font-medium">3</Table.Cell>
						<Table.Cell>Row 1</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell class="text-left">cell</Table.Cell>
						<Table.Cell> cell</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell class="text-right">
							<Button variant="destructive">Button</Button>
						</Table.Cell>
					</Table.Row>
					<Table.Row class=" border-slate-400 border-b">
						<Table.Cell class="font-medium">4</Table.Cell>
						<Table.Cell>Row 1</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell class="text-left">cell</Table.Cell>
						<Table.Cell> cell</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell class="text-right">
							<Button variant="destructive">Button</Button>
						</Table.Cell>
					</Table.Row>
					<Table.Row class=" border-slate-400 border-b">
						<Table.Cell class="font-medium">5</Table.Cell>
						<Table.Cell>Row 1</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell class="text-left">cell</Table.Cell>
						<Table.Cell> cell</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell class="text-right">
							<Button variant="destructive">Button</Button>
						</Table.Cell>
					</Table.Row>
					<Table.Row class=" border-slate-400 border-b">
						<Table.Cell class="font-medium">6</Table.Cell>
						<Table.Cell>Row 1</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell class="text-left">cell</Table.Cell>
						<Table.Cell> cell</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell class="text-right">
							<Button variant="destructive">Button</Button>
						</Table.Cell>
					</Table.Row>
					<Table.Row class=" border-slate-400 border-b">
						<Table.Cell class="font-medium">7</Table.Cell>
						<Table.Cell>Row 1</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell class="text-left">cell</Table.Cell>
						<Table.Cell> cell</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell class="text-right">
							<Button variant="destructive">Button</Button>
						</Table.Cell>
					</Table.Row>
					<Table.Row class=" border-slate-400 border-b-4">
						<Table.Cell class="font-medium">8</Table.Cell>
						<Table.Cell>Row 1</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell class="text-left">cell</Table.Cell>
						<Table.Cell> cell</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell>cell</Table.Cell>
						<Table.Cell class="text-right">
							<Button variant="destructive">Button</Button>
						</Table.Cell>
					</Table.Row>
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
