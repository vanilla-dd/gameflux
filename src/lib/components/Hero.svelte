<script lang="ts">
	import { Button } from './ui/button';
	import TournamentSection from './TournamentSection.svelte';
	import Marquee from './Marquee.svelte';
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
		'valorant.svg',
	];
</script>

<div class="mt-10 flex flex-col items-center gap-3 text-center">
	<h1 class="max-w-[30ch] text-7xl font-bold">Create your team and win tournaments now!</h1>
	<p class="max-w-[120ch] text-base">
		Lorem ipsum dolor sit amet consectetur, adipisicing elit. Laboriosam in ex eum harum eveniet
		minus nostrum suscipit sapiente eaque distinctio. Lorem ipsum, dolor sit amet consectetur
		adipisicing elit. Accusantium, voluptate? Quasi illo modi, velit quia sit quas fuga corrupti
		aliquid
	</p>
	<div>
		<Button variant="secondary">Discover Tournament</Button>
		<Button variant="outline">Create An Account</Button>
	</div>
	<div>
		<Marquee {images} />
	</div>
	<TournamentSection />
</div>
