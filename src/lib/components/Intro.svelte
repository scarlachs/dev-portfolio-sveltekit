<script>
	import ButtonGroup from "./ButtonGroup.svelte";
	import { buttonVariants } from "./ui/button";
	import Section from "./Section.svelte";
</script>

<Section class="pt-12 md:pt-16">
	<div class="relative md:flex md:items-center md:justify-center md:gap-10">
		<div class="max-md:mb-8 md:w-6/12 xl:w-5/12">
			<h1 class="mb-5 text-4xl font-bold max-md:pe-24 lg:text-5xl">Frontend-Entwickler</h1>
			<p class="mb-10 text-lg sm:max-lg:w-10/12 xl:w-11/12">
				Moin! Und willkommen in meiner Welt des Codes! Ich bin Frontend-Entwickler und zeige
				hier eine Auswahl meiner bisherigen Projekte.
			</p>
			<ButtonGroup>
				<a href="/#projects" class={buttonVariants({ variant: "default" })}
					>Aktuelle Projekte</a
				>
				<a href="/#about" class={buttonVariants({ variant: "secondary" })}>Über mich</a>
			</ButtonGroup>
		</div>
		<div class="w-9/12 md:w-6/12 xl:w-5/12">
			<enhanced:img
				src="$lib/images/Frontend-Developer-Pascal-Schaar.jpg?w=257;557;1154"
				alt="Ein Portrait von Pascal Schaar"
				class="img-mask h-auto w-full"
				sizes="(max-width: 639.98px) calc((100vw - 2rem) * 0.75), (max-width: 767.98px) 432px, (max-width: 1023.98px) 332px, (max-width: 1279.98px) 460px, (max-width: 1399.98px) 506px, 556px"
			/>
		</div>
	</div>
</Section>

<style lang="postcss">
	.img-mask {
		mask-image: url($lib/images/blob.svg);
		mask-repeat: no-repeat;
		mask-size: 100% 100%;
		@apply [mask-position:-1rem_center] md:[mask-position:-1.5rem_center];
	}
</style>
