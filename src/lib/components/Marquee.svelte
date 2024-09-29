<script lang="ts">
	import { Marquee } from '@selemondev/svelte-marquee';
	import '@selemondev/svelte-marquee/dist/style.css';
	export let images;
</script>

<Marquee direction="left" fade={true} reverse={false} innerClassName={'gap-10'} pauseOnHover={true}>
	{#each images as image}
		<img src={`/${image}`} alt="" class="w-36 object-contain" />
	{/each}
</Marquee>
