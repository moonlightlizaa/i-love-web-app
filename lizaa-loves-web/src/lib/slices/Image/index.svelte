<script>
	/** @type {import("@prismicio/client").Content.ImageSlice} */
	export let slice;

	import { PrismicImage } from "@prismicio/svelte";
</script>

<section class="image">
	<PrismicImage field={slice.primary.image} width="220px" />
</section>

<section class="spotify">
	<iframe style="border-radius:12px" src="https://open.spotify.com/embed/album/2fYhqwDWXjbpjaIJPEfKFw?utm_source=generator" width="100%" height="352" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
</section>

<style>

	.image {
		padding: 30px;
		margin: 30px 0px;
		border-radius: 26px;

		display: flex;
		justify-content: center;
		align-items: center;
	}

</style>