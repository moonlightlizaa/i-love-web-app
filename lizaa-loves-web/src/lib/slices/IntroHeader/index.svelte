<script>
	/** @type {import("@prismicio/client").Content.IntroHeaderSlice} */
	export let slice;


	import { PrismicRichText } from '@prismicio/svelte';
	import Label from './Label.svelte';

</script>


<header>
		<section class="header-title">
			{slice.primary.title}
		</section>

		<section class="header-text">
			<PrismicRichText field={slice.primary.text} />
		</section>
</header>

<style>


	header {
		background-color: #F6ECEF;
		padding: 30px;

		border-radius: 26px;
		margin-top: 100px;
	}

	.header-title {
		color: #5C3D4D;
		font-family: Quincy CF;
		font-size: 40px;
		font-style: normal;
		font-weight: 500;
		line-height: 120%; /* 48px */

		margin-bottom: 0.5em;
	}

	.header-text {
		color: #5C3D4D;
		font-family: Montserrat;
		font-size: 16px;
		font-style: normal;
		font-weight: 400;
		line-height: 150%; /* 24px */

		border-top: 0.5px solid #5C3D4D;
		padding: 0.7em;
	}
</style>