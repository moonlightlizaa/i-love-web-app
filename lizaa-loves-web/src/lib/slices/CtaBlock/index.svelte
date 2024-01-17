<script>
	/** @type {import("@prismicio/client").Content.AboutMeSlice} */
	export let slice;

	import { PrismicRichText } from '@prismicio/svelte';
	import {PrismicLink} from '@prismicio/svelte';
</script>

<article class="article-preview">
	<section class="title">
		{slice.primary.title}
	</section>
	<section class="text">
		<PrismicRichText field={slice.primary.text} />
	</section>
	<section class="cta-button">
		<PrismicLink field={slice.primary.link}>{slice.primary.label}</PrismicLink>
	</section>
</article>

<style>


:root {
				--primary-background-color:  #F9F6F7;
				--darker-background-color: #F6ECEF;
				--primary-white: #FFFFFF;
				--primary-pink: #F3B0C3;
				--primary-text-color: #5C3D4D;
			}
	

	.article-preview {
		padding: 30px;
		margin: 30px 0px;
		border-radius: 26px;
		background-color:var(--darker-background-color);
	}

	.title {
		color: var(--primary-text-color);
		font-family: Quincy CF;
		font-size: 22px;
		font-style: normal;
		font-weight: 600;

		padding-bottom: 0.8em;
	}

	.text {
		color: #5C3D4D;
		font-size: 1em;
		font-style: normal;
		font-weight: 400;

		padding-bottom: 1em;
		border-top: 0.5px solid #5C3D4D;
		padding-top: 1em;
	}

	.cta-button {
		background-color: var(--primary-pink);
		width: 100%;
		padding: 15px 30px;
		text-align: center;

		text-decoration: none;
		font-style: normal;
		font-weight: 600;
		font-size: 14px;

		display: flex;
		align-items: center;
		justify-content: center;

		border-radius: 15px;
	}



</style>