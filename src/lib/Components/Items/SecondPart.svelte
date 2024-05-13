<script>
	export let imageurl;
	export let name;
	export let description;
	export let arrow;
</script>

{#if arrow}
	<div class=" flex h-fit w-fit flex-row p-2">
		<img src={imageurl} alt="" class="my-auto h-14 w-14" />
		<div class="flex-col items-center p-4">
			<h1 class="font-bold text-black">{name}</h1>
			<p class="text-slate-700">{description}</p>
		</div>
		<img src="Items/arrow.png" class="my-auto h-8 w-20" />
	</div>
{:else}
	<div class=" flex h-full w-fit flex-row p-2">
		<img src={imageurl} alt="" class="my-auto h-14 w-14" />
		<div class="flex-col items-center p-4">
			<h1 class="font-bold text-black">{name}</h1>
			<p class="text-slate-700">{description}</p>
		</div>
	</div>
{/if}
