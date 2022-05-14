<script lang="ts">
	import { selected } from './selected';

	/**
	 * Makes the tile semitransparent for debugging
	 */
	export let semiTransparent = false;
	/**
	 * Adjusts the size and position.
	 * top,left,width,height
	 */
	export let data: string;
	/**
	 * Which organelle it corresponds to (for highlighting)
	 */
	export let title: string;
	/**
	 * Border radius of the tile (in px)
	 */
	export let rounded: string = '0';
	/**
	 * Degree of rotation (in degrees)
	 */
	export let rotation: string = '0';

	const parsedData = data.replace(/\s/g, '').split(',');
</script>

<div
	on:mouseenter={() => {
		selected.set(title);
	}}
	style="background: {semiTransparent ? 'rgb(0 0 0 / 55%)' : '#0000'}; top: {parsedData[0] + 'px' ??
		0}; left: {parsedData[1] + 'px' ?? 0}; width: {parsedData[2] + 'px' ??
		0}; height: {parsedData[3] + 'px' ??
		0}; position: absolute; border-radius: {rounded}px; transform: rotate({rotation}deg);"
/>
