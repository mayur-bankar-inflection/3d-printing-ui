<script>
	export let imageurl;
	export let name;
	export let description;
	export let arrow;
</script>

{#if arrow}
	<div class=" h-fit w-fit p-2 flex flex-row">
		<img src={imageurl} alt="" class="h-14 w-14 my-auto"/>
		<div class="flex-col items-center p-4">
			<h1 class="font-bold text-black">{name}</h1>
			<p class="text-slate-700">{description}</p>
		</div>
		<img src="arrow.png" class="h-8 w-20 my-auto" />
	</div>
{:else}
	<div class=" h-full w-fit p-2 flex flex-row ">
		<img src={imageurl} alt="" class="h-14 w-14 my-auto"/>
		<div class="flex-col items-center p-4">
			<h1 class="font-bold text-black">{name}</h1>
			<p class="text-slate-700">{description}</p>
		</div>
	</div>
{/if}