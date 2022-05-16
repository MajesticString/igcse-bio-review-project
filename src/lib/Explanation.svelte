<script lang="ts">
	import { selected } from '$lib/selected';

	/**
	 * The big text. Required for the hover thingy
	 */
	export let title: string;
</script>

<section
	class="my-2 prose border-[1px] p-3 rounded-xl {$selected === title ? 'shadow-xl shadow-indigo-500/50 bg-indigo-100' : 'border-slate-300'}"
>
	<h2>{title}</h2>
	<p><slot /></p>
</section>
