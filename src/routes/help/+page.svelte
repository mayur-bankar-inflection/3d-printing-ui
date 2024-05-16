<script lang="ts">
	import Button from '$lib/Components/ui/button/button.svelte';
	import { Input } from '$lib/components/ui/input/index.js';
	import { Label } from '$lib/components/ui/label/index.js';
	import { Textarea } from '$lib/components/ui/textarea/index.js';
</script>

<div class="m-2 mx-auto mt-8 max-w-lg p-8">
	<form class="mx-auto">
		<div class="w-full py-2">
			<div class="relative">
				<div class="flex w-full flex-col gap-1.5">
					<Label for="firstName" class="text-lg leading-7 text-gray-900">First Name</Label>
					<Input type="text" id="firstname" placeholder="First Name" class="w-full" />
				</div>
			</div>
		</div>
		<div class="w-full py-2">
			<div class="relative">
				<div class="flex w-full flex-col gap-1.5">
					<Label for="lastname" class="text-lg leading-7 text-gray-900">Last Name</Label>
					<Input type="text" id="lastname" placeholder="Last Name" />
				</div>
			</div>
		</div>
		<div class="w-full py-2">
			<div class="relative">
				<div class="flex w-full flex-col gap-1.5">
					<Label for="email" class="text-lg leading-7 text-gray-900">Email</Label>
					<Input type="email" id="email" placeholder="Email" />
				</div>
			</div>
		</div>

		<div class="w-full py-2">
			<div class="relative">
				<div class="flex w-full flex-col gap-1.5">
					<Label for="textarea" class="text-lg leading-7 text-gray-900">Message</Label>
					<Textarea placeholder="Type your message here." />
				</div>
			</div>
		</div>

		<Button class="my-2  w-full  ">Send</Button>
	</form>
</div>
