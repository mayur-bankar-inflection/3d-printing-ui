<script type="ts">
	import { Skeleton } from '$lib/components/ui/skeleton/index.ts';
</script>

<!-- svelte-ignore a11y-distracting-elements -->
<div class=" mx-auto my-20 h-80 w-fit bg-zinc-200 px-5 sm:h-fit">
	<div class="mt-5 flex w-full justify-center pt-5 text-2xl font-bold">
		<p class="  text-zinc-800">COLLABORATIONS</p>
	</div>
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
