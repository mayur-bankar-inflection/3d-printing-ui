<script lang="ts">
	import Button from '$lib/Components/ui/button/button.svelte';
	import { Input } from '$lib/components/ui/input/index.js';
	import { Label } from '$lib/components/ui/label/index.js';
	import { Textarea } from '$lib/components/ui/textarea/index.js';
</script>

<div class="mx-auto mt-8 max-w-lg p-8  m-2">
	<form class=" mx-auto">
		<div class="w-full p-2">
			<div class="relative">
				<div class="flex w-full max-w-sm flex-col gap-1.5">
					<Label for="firstName" class="text-lg leading-7 text-gray-900">First Name</Label>
					<Input type="text" id="firstname" placeholder="First Name" class="w-full"/>
				</div>
				<!-- <label for="name" class="py-4 text-lg leading-7 text-gray-900">First Name</label>
				<input
					type="text"
					id="firstname"
					name="firstname"
					placeholder="first name"
					required
					class=" w-full rounded border border-gray-400 bg-white px-1 py-1 text-base leading-8 text-gray-900 outline-none transition-colors duration-200 ease-in-out focus:border-blue-500 focus:bg-white focus:ring-2 focus:ring-blue-200"
				/> -->
			</div>
		</div>
		<div class="w-full p-2">
			<div class="relative">
				<div class="flex w-full max-w-sm flex-col gap-1.5">
					<Label for="lastname" class=" text-lg leading-7 text-gray-900">Last Name</Label>
					<Input type="text" id="lastname" placeholder="Last Name" />
				</div>
				<!-- <label for="lastname" class="py-4 text-lg leading-7 text-gray-900">Last Name</label>
				<input
					type="text"
					id="lastname"
					name="lastname"
					placeholder="last name"
					required
					class=" w-full rounded border border-gray-400 bg-white px-1 py-1 text-base leading-8 text-gray-900 outline-none transition-colors duration-200 ease-in-out focus:border-blue-500 focus:bg-white focus:ring-2 focus:ring-blue-200"
				/> -->
			</div>
		</div>
		<div class="w-full p-2">
			<div class="relative">
				<div class="flex w-full max-w-sm flex-col gap-1.5">
					<Label for="email" class=" text-lg leading-7 text-gray-900">Email</Label>
					<Input type="email" id="email" placeholder="email" />
				</div>
				<!-- <label for="email" class="py-4 text-lg leading-7 text-gray-900">Email</label>
				<input
					type="email"
					id="email"
					name="email"
					placeholder="abc@gmail.com"
					required
					class=" w-full rounded border border-gray-400 bg-white px-1 py-1 text-base leading-8 text-gray-900 outline-none transition-colors duration-200 ease-in-out focus:border-blue-500 focus:bg-white focus:ring-2 focus:ring-blue-200"
				/> -->
			</div>
		</div>

		<div class="w-full p-2">
			<div class="relative">
				<div class="flex w-full max-w-sm flex-col gap-1.5">
					<Label for="textarea" class=" text-lg leading-7 text-gray-900">Message</Label>
					<Textarea placeholder="Type your message here." class="w-full"/>
				</div>
				<!-- <label for="message" class="py-4 text-lg leading-7 text-gray-900">Message</label>
				<textarea
					id="message"
					name="message"
					placeholder="type here.."
					required
					class=" h-32 w-full resize-none rounded border border-gray-400 bg-white px-3 py-1 text-base leading-6 text-gray-900 outline-none transition-colors duration-200 ease-in-out focus:border-blue-500 focus:bg-white focus:ring-2 focus:ring-blue-200"
				></textarea> -->
			</div>
		</div>
		<div class="w-full p-2">
			<Button
				type="submit"
				class="mx-auto flex  rounded  px-20 py-2 text-lg font-semibold text-white hover:bg-black"
				>Submit</Button
			>
		</div>
	</form>
</div>
