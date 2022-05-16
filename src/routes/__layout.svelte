<script lang="ts">
	import { onMount } from 'svelte';
	import {
		Dialog,
		DialogOverlay,
		DialogTitle,
		Transition,
		TransitionChild,
	} from '@rgossiaux/svelte-headlessui';

	let isDialogOpen = false;

	// device detection
	onMount(() => {
		if (window.innerWidth < 700 && !localStorage.getItem('isMobileDialog')) {
			openModal();
			localStorage.setItem('isMobileDialog', 'true');
		}
	});

	function closeModal() {
		isDialogOpen = false;
	}
	function openModal() {
		isDialogOpen = true;
	}
</script>

<Transition appear show={isDialogOpen}>
	<Dialog as="div" class="fixed inset-0 z-10 overflow-y-auto" on:close={closeModal}>
		<div class="min-h-screen px-4 text-center">
			<TransitionChild
				enter="ease-out duration-300"
				enterFrom="opacity-0"
				enterTo="opacity-100"
				leave="ease-in duration-200"
				leaveFrom="opacity-100"
				leaveTo="opacity-0"
			>
				<DialogOverlay class="fixed inset-0" />
			</TransitionChild>

			<TransitionChild
				enter="ease-out duration-300"
				enterFrom="opacity-0 scale-95"
				enterTo="opacity-100 scale-100"
				leave="ease-in duration-200"
				leaveFrom="opacity-100 scale-100"
				leaveTo="opacity-0 scale-95"
			>
				<!-- This element is to trick the browser into centering the modal contents. -->
				<span class="inline-block h-screen align-middle" aria-hidden="true"> &#8203; </span>
				<div
					class="inline-block w-full max-w-md p-6 my-8 overflow-hidden text-left align-middle transition-all transform bg-white shadow-xl rounded-2xl"
				>
					<DialogTitle as="h3" class="text-lg font-medium leading-6 text-gray-900">
						This site looks terrible on mobile.
					</DialogTitle>
					<div class="mt-2">
						<p class="text-sm text-gray-500">
							Images look like a literal dot; try using a desktop.
						</p>
					</div>

					<div class="mt-4">
						<button
							type="button"
							class="inline-flex justify-center px-4 py-2 text-sm font-medium text-blue-900 bg-blue-100 border border-transparent rounded-md hover:bg-blue-200 focus:outline-none focus-visible:ring-2 focus-visible:ring-offset-2 focus-visible:ring-blue-500"
							on:click={closeModal}
						>
							Ignore Advice
						</button>
					</div>
				</div>
			</TransitionChild>
		</div>
	</Dialog>
</Transition>

<div class="top-0 mb-4 px-6 text-xl text-black w-full border-b z-20">
	<div class="py-4 pr-4 flex justify-between items-center">
		<div class="flex items-center space-x-4 md:space-x-0">
			<a href="/">
				<span class="text-blue-600 font-bold">Cell Structures</span> Biology Review Project
			</a>
		</div>

		<div class="flex-grow" />

		<a class="mx-2" href="/animal-cell">Animal Cell</a>
		<a class="mx-2" href="/plant-cell">Plant Cell</a>
		<!-- <a class="mx-2" href="/bacteria-cell">Bacteria Cell</a> -->
	</div>
</div>

<slot />

<style lang="scss">
	@import 'tailwindcss/base';
	@import 'tailwindcss/components';
	@import 'tailwindcss/utilities';
</style>
