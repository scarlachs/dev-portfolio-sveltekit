<script lang="ts">
	import type { SVGAttributes } from "svelte/elements";
	import { cn } from "$lib/ts/utils";

	type $$Props = SVGAttributes<SVGElement>;
</script>

<svg
	xmlns="http://www.w3.org/2000/svg"
	width="256"
	height="256"
	viewBox="0 0 256 256"
	fill="none"
	aria-labelledby="shadcn"
	{...$$restProps}
	class={cn($$restProps.class, "text-zinc-950 dark:text-zinc-50")}
>
	<title id="shadcn">shadcn/ui</title>
	<line
		x1="208"
		y1="128"
		x2="128"
		y2="208"
		fill="none"
		stroke="currentColor"
		stroke-linecap="round"
		stroke-linejoin="round"
		stroke-width="16"
	></line>
	<line
		x1="192"
		y1="40"
		x2="40"
		y2="192"
		fill="none"
		stroke="currentColor"
		stroke-linecap="round"
		stroke-linejoin="round"
		stroke-width="16"
	></line>
</svg>
