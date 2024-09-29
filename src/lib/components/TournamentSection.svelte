<script lang="ts">
	import { CalendarClock, Trophy, User, UserRoundSearch } from 'lucide-svelte';
	import { Separator } from './ui/separator';
	import { Button } from './ui/button';
	const tournamentDetails = [
		{
			id: 'idkwhatever',
			image: '/fortnite-match.png',
			time: new Date(),
			name: 'Fortnite: Platinum Tournament',
			tags: ['free', 'fortnite', 'PC'],
			event: {
				prizePool: 400,
				currency: 'USD',
				teamSize: 4,
				totalSeats: 100,
				filledSeats: 14,
			},
		},
		{
			id: 'idkwhatever1',
			image: '/pubg-match.png',
			time: new Date(),
			name: 'Pubg: Elite Cup',
			tags: ['free', 'pubg', 'mobile'],
			event: {
				prizePool: 4000,
				currency: 'USD',
				teamSize: 4,
				totalSeats: 100,
				filledSeats: 96,
			},
		},
		{
			id: 'idkwhatever2',
			image: '/fortnite-match.png',
			time: new Date(),
			name: 'Fortnite: Rookie Tournament',
			tags: ['free', 'fortnite', 'PC'],
			event: {
				prizePool: 40,
				currency: 'USD',
				teamSize: 4,
				totalSeats: 100,
				filledSeats: 24,
			},
		},

		{
			id: 'idkwhatever3',
			image: '/among-us-match.png',
			time: new Date(),
			name: 'Among Us: Fun Play',
			tags: ['free', 'AmongUs', 'PC', 'Mobile'],
			event: {
				prizePool: 0,
				currency: 'USD',
				teamSize: 1,
				totalSeats: 140,
				filledSeats: 14,
			},
		},
	];
</script>

<div class="flex flex-col gap-8 px-8">
	<p class="text-5xl font-semibold underline decoration-dashed underline-offset-4">Tournament</p>
	<div class="flex flex-wrap justify-center gap-4">
		{#each tournamentDetails as tournament}
			<div class="w-80 space-y-3 rounded-md p-2 outline outline-gray-200">
				<img
					src={tournament.image}
					alt="tournament logo"
					class="aspect-video w-full rounded-md object-cover object-top"
				/>
				<div class="space-y-4 px-1">
					<div>
						<p class="flex items-center gap-2 text-sm">
							<CalendarClock class="w-5" />
							Sept 1 • 9:00AM EST
						</p>
						<p class="text-start text-xl font-semibold capitalize">{tournament.name}</p>
					</div>
					<div class="space-y-2">
						<div class="flex flex-wrap gap-2 text-xs text-black/70">
							{#each tournament.tags as tag}
								<p
									class="rounded-sm bg-gray-100 px-3 py-0.5 capitalize outline outline-1 outline-black/40"
								>
									{tag}
								</p>
							{/each}
						</div>
						<div class="flex justify-between gap-2 text-black/70">
							<p>
								Prize pool
								<span class="flex items-center justify-center gap-1 font-medium"
									><Trophy class="w-5" />${tournament.event.prizePool}</span
								>
							</p>
							<Separator orientation="vertical" class="my-3" />
							<p>
								Team size
								<span class="flex items-center justify-center gap-1 font-medium"
									><User class="w-5" />{tournament.event.teamSize}v{tournament.event.teamSize}</span
								>
							</p>
							<Separator orientation="vertical" class="my-3" />
							<p>
								Participants
								<span class="flex items-center justify-center gap-1 font-medium"
									><UserRoundSearch class="w-5" />{tournament.event.filledSeats}/{tournament.event
										.totalSeats}</span
								>
							</p>
						</div>
					</div>
					<div class="flex justify-between gap-4">
						<!-- <div class="flex flex-shrink-0 items-center justify-between gap-2">
                        <p>Organized by:</p>
                        <a href="/user/user_id">
                            <img src="https://placehold.co/24" alt="" class="rounded-full" /></a
                        >
                    </div> -->
						<a href={`/tournament/${tournament.id}`} class="w-full">
							<Button variant="outline" class="w-full">Join Tournament</Button>
						</a>
					</div>
				</div>
			</div>
		{/each}
	</div>
	<a href="/events" class="self-center rounded-md">
		<Button>Discover more</Button>
	</a>
</div>
