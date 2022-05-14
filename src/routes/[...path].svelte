<script context="module" lang="ts">
	import type { Load } from '@sveltejs/kit';

	export const load: Load = ({ params }) => {
		return {
			status: 404,
			error: new Error(`Not found: /${params.path}`),
		};
	};
</script>
