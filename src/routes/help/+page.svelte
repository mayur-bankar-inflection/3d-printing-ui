<script>
	import Button from "$lib/Components/ui/button/button.svelte";

</script>
<div class="mx-auto mt-8 max-w-lg p-8">
	<form>
		<div class="w-full p-2">
			<div class="relative">
				<label for="name" class="py-4 text-lg leading-7 text-gray-900">First Name</label>
				<input
					type="text"
					id="firstname"
					name="firstname"
					placeholder="first name"
					required
					class=" w-full rounded border border-gray-400 bg-white px-1 py-1 text-base leading-8 text-gray-900 outline-none transition-colors duration-200 ease-in-out focus:border-blue-500 focus:bg-white focus:ring-2 focus:ring-blue-200"
				/>
			</div>
		</div>
		<div class="w-full p-2">
			<div class="relative">
				<label for="lastname" class="py-4 text-lg leading-7 text-gray-900">Last Name</label>
				<input
					type="text"
					id="lastname"
					name="lastname"
					placeholder="last name"
					required
					class=" w-full rounded border border-gray-400 bg-white px-1 py-1 text-base leading-8 text-gray-900 outline-none transition-colors duration-200 ease-in-out focus:border-blue-500 focus:bg-white focus:ring-2 focus:ring-blue-200"
				/>
			</div>
		</div>
		<div class="w-full p-2">
			<div class="relative">
				<label for="email" class="py-4 text-lg leading-7 text-gray-900">Email</label>
				<input
					type="email"
					id="email"
					name="email"
					placeholder="abc@gmail.com"
					required
					class=" w-full rounded border border-gray-400 bg-white px-1 py-1 text-base leading-8 text-gray-900 outline-none transition-colors duration-200 ease-in-out focus:border-blue-500 focus:bg-white focus:ring-2 focus:ring-blue-200"
				/>
			</div>
		</div>

		<div class="w-full p-2">
			<div class="relative">
				<label for="message" class="py-4 text-lg leading-7 text-gray-900">Message</label>
				<textarea
					id="message"
					name="message"
					placeholder="type here.."
					required
					class=" h-32 w-full resize-none rounded border border-gray-400 bg-white px-3 py-1 text-base leading-6 text-gray-900 outline-none transition-colors duration-200 ease-in-out focus:border-blue-500 focus:bg-white focus:ring-2 focus:ring-blue-200"
				></textarea>
			</div>
		</div>
		<div class="w-full p-2">
			<Button
				type="submit"
				class="w-full rounded  px-4 py-2 text-lg font-semibold text-white hover:bg-black"
				>Submit</Button
			>
		</div>
	</form>
</div>
