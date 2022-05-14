<script lang="ts">
	import Explanation from '$lib/Explanation.svelte';
</script>

<svelte:head>
	<title>Plant Cell - Cell Structures Review Project</title>
</svelte:head>
<div class="w-full text-center prose flex justify-center mx-auto mb-4">
	<h1 class="w-full text-center justify-self-center">Plant Cell</h1>
</div>
<div class="flex flex-row mx-8">
	<div class="flex flex-col left-explanations">
		<Explanation title="Cell Wall">
			A structural, often firm layer surrounding the cell membrane that keeps the plant cells shape,
			and protects the cell.
		</Explanation>
		<Explanation title="Vacuole"
			>The vacuole contains mostly water. Stores waste. Typically takes up around 80% of the cells
			volume. Helps to support the cell wall.</Explanation
		>
		<Explanation title="Mitochondria">
			Also known as the powerhouse the cell. Uses aerobic respiration to produce chemical energy.
		</Explanation>
		<Explanation title="Chloroplasts">
			Chloroplasts contain chlorophyll, and are the place where photosynthesis takes place.
		</Explanation>
		<Explanation title="Ribosomes">
			Contains RNA. Also synthesizes proteins from amino acids.
		</Explanation>
	</div>
	<div class="image relative w-[700px]">
		<img src="/plant-cell.png" alt="Plant Cell" />
	</div>
	<div class="right-explanations">
		<Explanation title="Cell Membrane">
			Also called the "plasma membrane" or "cytoplasmic membrane." The plasma membrane separates the
			innards of the cell from the outside world.
		</Explanation>
		<Explanation title="Smooth Endoplasmic Reticulum">
			Synthesizes lipids, and phospholipids (which form the cell membrane). Helps to metabolize
			carbohydrates. Does not contain ribosomes on its surface.
		</Explanation>
		<Explanation title="Rough Endoplasmic Reticulum">
			Synthesizes lipids and proteins. Contains ribosomes on its surface.
		</Explanation>
	</div>
</div>
