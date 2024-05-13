<script lang="ts">
	import { AspectRatio } from '$lib/components/ui/aspect-ratio';
</script>

<div class="space-y-4">
	<!-- <img src="items/cube.png" alt="3D printing UI" class="mx-auto h-[200px] w-[300px]" /> -->
	<div class="mx-auto w-[450px]">
		<AspectRatio ratio={16 / 9} class="bg-muted">
			<img src="Items/OIP.jpg" alt="..." class="mx-auto h-full w-full rounded-md object-cover" />
		</AspectRatio>
	</div>
	<!-- <img src="items/logo-select.svg" alt="Logo image" class="mx-auto h-10" /> -->
	<p class="mx-auto text-pretty text-center text-slate-800 sm:px-[20%] md:px-[40%]">
		Lorem ipsum dolor sit amet consectetur adipisicing elit. Repudiandae voluptas quidem sunt nulla
		rerum quisquam quibusdam fugiat corrupti eaque non minima voluptates sint tempore, fugit ut
		illum dicta officia itaque!
	</p>
	<a href="www.google.com" class="mx-auto flex justify-center text-2xl text-blue-500 underline"
		>Learn More</a
	>
</div>
