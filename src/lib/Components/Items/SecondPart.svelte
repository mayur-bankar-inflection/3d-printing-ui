<script>
	export let imageurl;
	export let name;
	export let description;
	export let arrow;
</script>

{#if arrow}
	<div
		class="m-4 flex flex-row space-x-4 bg-gradient-to-r from-violet-500 to-violet-300 p-2 duration-300 hover:scale-110 hover:shadow-2xl"
	>
		<img src={imageurl} alt="" class="my-auto h-14 w-14" />
		<div class="flex flex-col items-center p-4">
			<h1 class="font-bold text-black">{name}</h1>
			<p class="text-slate-700">{description}</p>
		</div>
		<img src="Items/arrow.png" class="my-auto h-8 w-20" />
	</div>
{:else}
	<div
		class="m-4 flex flex-row space-x-2 bg-gradient-to-r from-violet-500 to-violet-300 p-2 duration-300 hover:scale-110 hover:shadow-2xl"
	>
		<img src={imageurl} alt="" class="my-auto h-14 w-14" />
		<div class="flex flex-col items-center p-4">
			<h1 class="font-bold text-black">{name}</h1>
			<p class="text-slate-700">{description}</p>
		</div>
	</div>
{/if}
