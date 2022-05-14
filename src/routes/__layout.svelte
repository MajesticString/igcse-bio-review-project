<div class="sticky top-0 mb-4 px-6 text-xl text-black w-full backdrop-blur border-b z-20">
	<div class="py-4 pr-4 flex justify-between items-center">
		<div class="flex items-center space-x-4 md:space-x-0">
			<a href="/">
				<span class="text-blue-600">Biology</span> Review Project
			</a>
		</div>

		<div class="flex-grow" />

		<a class="mx-2" href="/animal-cell">Animal Cell</a>
		<a class="mx-2" href="/plant-cell">Plant Cell</a>
		<a class="mx-2" href="/bacteria-cell">Bacteria Cell</a>
	</div>
</div>

<slot />

<style lang="scss">
	@import 'tailwindcss/base';
	@import 'tailwindcss/components';
	@import 'tailwindcss/utilities';
</style>
