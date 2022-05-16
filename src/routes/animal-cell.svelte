<script lang="ts">
  import Explanation from "$lib/Explanation.svelte";
  import Tile from "$lib/Tile.svelte";
</script>

<svelte:head>
  <title>Animal Cell - Cell Structures Review Project</title>
</svelte:head>

<div class="w-full text-center flex-col prose flex justify-center mx-auto mb-4">
  <h1 class="w-full m-2 text-center justify-self-center">Animal Cell</h1>
  <p class="w-full m-2 text-center justify-self-center">
    Hover over the cell structures to highlight the definition
  </p>
</div>
<div class="flex flex-row mx-8">
  <div class="flex flex-col left-explanations">
    <Explanation title="Vacuole">
      The vacuole contains mostly water. Stores waste. Not as large in animal
      cells.
    </Explanation>
    <Explanation title="Mitochondria">
      Also known as the powerhouse the cell. Uses aerobic respiration to produce
      chemical energy.
    </Explanation>
    <Explanation title="Ribosomes">
      <b>(the little brown specs everywhere that im too lazy to highlight)</b>
      Contains RNA. Also synthesizes proteins from amino acids.
    </Explanation>
    <Explanation title="Cytoplasm">
      A gelatinous liquid that fills up a majority of the cell (apart from the
      vacuole). Mainly consists of water.
    </Explanation>
    <Explanation title="Lysosomes">
      Contains digestive enzymes, and rids waste products.
    </Explanation>
    <Explanation title="Peroxisomes">
      Contains enzymes. Carries out oxidative reactions. Generates hydrogen
      peroxide for those reactions.
    </Explanation>
  </div>
  <div class="fixed top-4 w-[700px] min-w-[700px]">
    <div class="image relative w-full">
      <img src="/animal-cell.png" alt="Animal Cell" />
      <Tile title="Cell Membrane" data="10,10,680,670" rounded="340" />
      <Tile title="Cytoplasm" data="30,30,640,630" rounded="340" />
      <Tile
        title="Mitochondria"
        data="270,77,45,100"
        rounded="90"
        rotation="54"
      />
      <Tile
        title="Mitochondria"
        data="420,300,45,100"
        rounded="90"
        rotation="120"
      />
      <Tile title="Mitochondria" data="370,580,45,100" rounded="90" />
      <Tile title="Vacuole" data="390,140,90,130" rounded="100" />
      <Tile
        title="Rough Endoplasmic Reticulum"
        data="70,190,300,300"
        rounded="150"
      />
      <Tile title="Nucleus" data="130,280,170,170" rounded="90" />
      <Tile title="Nucleoid" data="220,360,50,50" rounded="90" />
      <Tile
        title="Smooth Endoplasmic Reticulum"
        data="60,180,70,120"
        rotation="18"
      />
      <Tile title="Golgi Apparatus" data="370,340,150,100" />
      <Tile title="Lysosomes" data="550,300,70,70" rounded="30" />
      <Tile title="Peroxisomes" data="160,130,50,50" rounded="25" />
      <Tile title="Peroxisomes" data="280,580,50,50" rounded="25" />
    </div>
  </div>
  <div class="right-explanations">
    <Explanation title="Cell Membrane">
      Also called the "plasma membrane" or "cytoplasmic membrane." The plasma
      membrane separates the innards of the cell from the outside world.
    </Explanation>
    <Explanation title="Smooth Endoplasmic Reticulum">
      Synthesizes lipids, and phospholipids (which form the cell membrane).
      Helps to metabolize carbohydrates. Does not contain ribosomes on its
      surface.
    </Explanation>
    <Explanation title="Rough Endoplasmic Reticulum">
      Synthesizes lipids and proteins. Contains ribosomes on its surface.
    </Explanation>
    <Explanation title="Nucleus">
      Controls the activities of the cell. ALso contains the cells DNA.
    </Explanation>
    <Explanation title="Nucleoid">
      Contains a majority of the genetic material. Controls the activity of the
      cell.
    </Explanation>
    <Explanation title="Golgi Apparatus">
      Helps process and package lipids and proteins from the endoplasmic
      reticulum into vesicles.
    </Explanation>
  </div>
</div>
