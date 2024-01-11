<script>
	import { PrismicRichText } from '@prismicio/svelte';
	import { PrismicImage } from '@prismicio/svelte';
	import {PrismicLink} from '@prismicio/svelte';
	import Label from './Label.svelte';

	/** @type {import("@prismicio/client").Content.HomeHeaderSlice} */
	export let slice;
</script>


<section class="header">
	<section class="header-intro">
			<section class="header-title">
				<PrismicRichText field={slice.primary.header_title} />
			</section>
			<section class="header-text">
				<PrismicRichText field={slice.primary.header_text} />
			</section>
			<section class="header-button-portfolio"> 
				
			</section>
	</section>

	<section class="header-intro-img">
			<section class="header-image">
				<PrismicImage field={slice.primary.header_image} width="450px" />
			</section>
	</section>
</section>

<style>

	:root {
		--white: #FFFFFF;
		--background-color: #F9F6F7;
		--primary-text: #5C3D4D;
		--primary-pink: #F3B0C3;
	}

	.header {
		max-width: 1150px;
		margin: 0 auto;

		display: grid;
		grid: 
		"text image" 1fr
		/ 1fr 1fr;
		gap: 20px
	}

	.header-intro {
		grid-area: text;
	}

	.header-intro-img {
		grid-area: image;
	}

	.header-title {

		color: var(--primary-pink);
		font-family: Quincy CF;
		font-size: 3em;
		font-weight: 500;
		
	}

	.header-text {
		color: var(--primary-text);
		font-family: Montserrat;
		font-size: 1.1em;
		font-weight: 400;
		line-height: 150%; /* 27px */	
	}

	.header-image {
		width: 400px;
	}

	.header-button-portfolio a {
		background-color: var(--primary-pink);
		color: white;
		padding: 14px 25px;
		text-align: center;
		text-decoration: none;
		display: inline-block;

		color: var(white);
		font-family: Montserrat;
		font-size: 1em;
		font-weight: 600;
	}


</style>