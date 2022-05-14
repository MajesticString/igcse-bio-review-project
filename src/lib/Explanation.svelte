<script lang="ts">
	import { selected } from './selected';

	/**
	 * The big text. Required for the hover thingy
	 */
	export let title: string;
</script>

<section
	class="my-2 prose border-slate-300 border-[1px] p-3 rounded-xl"
	class:selected={$selected === title}
>
	<h2>{title}</h2>
	<p><slot /></p>
</section>

<style lang="scss">
	.selected {
		box-shadow: 0px 1px 2px rgba(0, 0, 0, 0.3), 0px 2px 6px 2px rgba(0, 0, 0, 0.15);
	}
</style>
