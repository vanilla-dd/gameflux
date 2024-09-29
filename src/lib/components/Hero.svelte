<script lang="ts">
	import { Marquee } from '@selemondev/svelte-marquee';
	import '@selemondev/svelte-marquee/dist/style.css';
	import { Button } from './ui/button';
	import { CalendarClock, Clock } from 'lucide-svelte';
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
	<div class="flex flex-col gap-8 px-8">
		<p class="text-5xl font-semibold underline decoration-dashed underline-offset-4">Tournament</p>
		<div class="flex flex-wrap justify-center gap-4">
			<div class="w-80 rounded-md p-2 outline outline-gray-200">
				<img
					src="/fortnite-match.png"
					alt=""
					class="aspect-video w-full rounded-md object-cover object-top"
				/>
				<div class="text-start">
					<p class="flex items-center gap-2 text-xs">
						<CalendarClock class="w-4" />
						Sept. 1 9:00AM EST
					</p>
					<p class="text-lg font-medium">Fortnite: Platinum Tournament</p>
					<div class="flex flex-wrap gap-2">
						<p class="rounded-sm bg-gray-100 px-2 text-xs outline outline-1 outline-black/40">PC</p>
						<p class="rounded-sm bg-gray-100 px-2 text-xs outline outline-1 outline-black/40">
							Fortnite
						</p>
						<p class="rounded-sm bg-gray-100 px-2 text-xs outline outline-1 outline-black/40">
							Free
						</p>
					</div>
					<div>
						<div>
							<p>
								Prize pool
								<span>$400</span>
							</p>
						</div>
						<div>
							<p>
								Team size
								<span>4v4</span>
							</p>
						</div>
						<div>
							<p>
								Participants
								<span>14/100</span>
							</p>
						</div>
					</div>
				</div>
				<div>
					<Button>Join Tournament</Button>
				</div>
			</div>
		</div>
	</div>
</div>
