<script>
	import * as Card from '$lib/components/ui/card';
</script>

<div class="w-full space-x-2  sm:w-auto sm:p-4 sm:py-6">
	<div
		class="w-full rounded-md shadow-md duration-300 hover:scale-110 hover:border-2 hover:border-violet-300 hover:shadow-2xl"
	>
		<Card.Root>
			<Card.Header>
				<Card.Title>Card Title</Card.Title>
				<Card.Description>Card Description</Card.Description>
			</Card.Header>
			<Card.Content>
				<p>
					Lorem ipsum dolor sit amet consectetur, adipisicing elit. Fugit doloremque adipisci
					ducimus ullam impedit, repellat amet atque quos aliquam nulla voluptates fuga nobis
					deleniti fugiat, sed voluptatibus quibusdam dicta. Saepe!
				</p>
			</Card.Content>
			<Card.Footer>
				<p>Card Footer</p>
			</Card.Footer>
		</Card.Root>
	</div>
</div>
