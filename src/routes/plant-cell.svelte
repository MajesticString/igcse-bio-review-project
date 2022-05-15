<script lang="ts">
	import Explanation from '$lib/Explanation.svelte';
	import Tile from '$lib/Tile.svelte';
</script>

<svelte:head>
	<title>Plant Cell - Cell Structures Review Project</title>
</svelte:head>
<div class="w-full flex-col text-center prose flex justify-center mx-auto mb-4">
	<h1 class="w-full m-2 text-center justify-self-center">Plant Cell</h1>

	<p class="w-full m-2 text-center justify-self-center">
		Hover over the cell structures to highlight the definition.
	</p>
</div>
<div class="flex flex-col md:flex-row mx-8">
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
			<b>(the little brown specs everywhere that im too lazy to highlight)</b> Contains RNA. Also synthesizes
			proteins from amino acids.
		</Explanation>
		<Explanation title="Cytoplasm">
			A gelatinous liquid that fills up a majority of the cell (apart from the vacuole). Mainly
			consists of water.
		</Explanation>
	</div>
	<div class="image relative w-[700px] min-w-[700px]">
		<img src="/plant-cell.png" alt="Plant Cell" />
		<Tile title="Cell Wall" data="20,20,660,640" />
		<Tile title="Cell Membrane" data="40,40,620,590" rounded="90" />
		<Tile title="Cytoplasm" data="60,60,570,550" rounded="90" />
		<Tile title="Mitochondria" data="55,87,45,100" rounded="90" rotation="54" />
		<Tile title="Mitochondria" data="410,87,45,100" rounded="90" rotation="110" />
		<Tile title="Mitochondria" data="450,565,45,100" rounded="90" rotation="54" />
		<Tile title="Chloroplasts" data="520,555,55,100" rounded="90" rotation="44" />
		<Tile title="Chloroplasts" data="520,80,55,100" rounded="90" rotation="120" />
		<Tile title="Chloroplasts" data="50,240,55,100" rounded="90" rotation="120" />
		<Tile title="Vacuole" data="100,100,210,250" rounded="100" rotation="150" />
		<Tile title="Vacuole" data="230,175,230,400" rounded="150" rotation="140" />
		<Tile title="Vacuole" data="230,105,230,200" rotation="-20" />
		<Tile title="Rough Endoplasmic Reticulum" data="70,340,284,270" rounded="135" />
		<Tile title="Nucleus" data="120,420,170,170" rounded="90" />
		<Tile title="Nucleoid" data="200,495,50,50" rounded="90" rotation="-90" />
		<Tile title="Smooth Endoplasmic Reticulum" data="60,315,70,120" rotation="18" />
		<Tile title="Golgi Apparatus" data="350,480,150,100" />
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
		<Explanation title="Nucleus">
			Controls the activities of the cell. ALso contains the cells DNA.
		</Explanation>
		<Explanation title="Nucleoid">
			Contains a majority of the genetic material. Controls the activity of the cell.
		</Explanation>
		<Explanation title="Golgi Apparatus">
			Helps process and package lipids and proteins from the endoplasmic reticulum into vesicles.
		</Explanation>
	</div>
</div>
