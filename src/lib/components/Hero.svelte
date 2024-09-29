<script lang="ts">
	import { Marquee } from '@selemondev/svelte-marquee';
	import '@selemondev/svelte-marquee/dist/style.css';
	import { Button } from './ui/button';
	const images = [
		'among-us.svg',
		'apex-legends.svg',
		'counter-strike.svg',
		'dota-2.svg',
		'fall-guys.svg',
		'fortnite.svg',
		// 'free-fire.svg',
		'league-of-legends.svg',
		'minecraft.svg',
		'mortal-kombat.svg',
		'overwatch.svg',
		'pubg.svg',
		'r6siege.svg',
		'rocket.svg',
		'valorant.svg'
	];
</script>

<div class="flex flex-col items-center gap-3 text-center">
	<h1 class="max-w-[30ch] text-7xl font-bold">Create your team and win tournaments now!</h1>
	<p class="max-w-[150ch] text-base">
		Lorem ipsum dolor sit amet consectetur, adipisicing elit. Laboriosam in ex eum harum eveniet
		minus nostrum suscipit sapiente eaque distinctio. Lorem ipsum, dolor sit amet consectetur
		adipisicing elit. Accusantium, voluptate? Quasi illo modi, velit quia sit quas fuga corrupti
		aliquid sapiente laboriosam, ad, deleniti dolores dolor recusandae minima impedit dignissimos!
	</p>
	<div>
		<Button variant="secondary">Discover Tournament</Button>
		<Button variant="outline">Create An Account</Button>
	</div>
	<div>
		<Marquee
			direction="left"
			fade={true}
			reverse={false}
			innerClassName={'gap-10'}
			pauseOnHover={true}
		>
			{#each images as image}
				<img src={`/${image}`} alt="" class="w-36 object-contain" />
			{/each}
		</Marquee>
	</div>
</div>
