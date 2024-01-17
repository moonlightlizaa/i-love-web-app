<script>
	import { SliceZone } from '@prismicio/svelte';

	import { components } from '$lib/slices';

	export let data;
</script>

<SliceZone slices={data.page.data.slices} {components} />

<!-- dit kom te zien op alle pagina's -->