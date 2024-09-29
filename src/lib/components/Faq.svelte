<script lang="ts">
	import * as Accordion from '$lib/components/ui/accordion/index.js';
</script>

<div class="px-8">
	<p class="text-4xl font-semibold">FAQ</p>
	<div>
		<Accordion.Root class="w-full">
			<Accordion.Item value="item-1">
				<Accordion.Trigger>Is GamerFlux a trusted site?</Accordion.Trigger>
				<Accordion.Content>
					Yes. GamerFlux is a secure and reliable platform that follows industry standards, ensuring
					a safe experience for all users. Our platform is built with security protocols in place to
					protect personal data and transactions.
				</Accordion.Content>
			</Accordion.Item>
			<Accordion.Item value="item-2">
				<Accordion.Trigger>How do winning cashouts work?</Accordion.Trigger>
				<Accordion.Content>
					Winning cashouts are processed securely through our payment partners. After winning a
					tournament, your earnings are automatically credited to your GamerFlux account. From
					there, you can request a withdrawal to your preferred payment method, which typically
					takes 1-3 business days to process.
				</Accordion.Content>
			</Accordion.Item>
			<Accordion.Item value="item-3">
				<Accordion.Trigger>How can I find teammates?</Accordion.Trigger>
				<Accordion.Content>
					You can find teammates by joining our community features like forums and team matchmaking
					services. You can also join a public tournament as a solo player and get paired with other
					players looking for teammates.
				</Accordion.Content>
			</Accordion.Item>
			<Accordion.Item value="item-4">
				<Accordion.Trigger>How can I create tournaments?</Accordion.Trigger>
				<Accordion.Content>
					Creating tournaments on GamerFlux is simple. Navigate to the "Host a Tournament" section,
					provide details such as game, rules, entry fee, and prizes. Once submitted, the tournament
					will be listed for players to join.
				</Accordion.Content>
			</Accordion.Item>
			<Accordion.Item value="item-6">
				<Accordion.Trigger>Are there any entry fees for tournaments?</Accordion.Trigger>
				<Accordion.Content>
					It depends on the tournament. Some tournaments are free to join, while others may require
					an entry fee. Entry fees are usually listed in the tournament details, and these fees
					contribute to the prize pool.
				</Accordion.Content>
			</Accordion.Item>
			<Accordion.Item value="item-7">
				<Accordion.Trigger>How are tournament winners decided?</Accordion.Trigger>
				<Accordion.Content>
					Winners are determined based on the specific rules of the tournament, which are set by the
					host. Most tournaments are structured with single or double elimination brackets. The
					tournament host or GamerFlux admins oversee the fairness and completion of each event.
				</Accordion.Content>
			</Accordion.Item>
			<Accordion.Item value="item-8">
				<Accordion.Trigger
					>How do I report issues or disputes during a tournament?</Accordion.Trigger
				>
				<Accordion.Content>
					If you experience any issues or disputes during a tournament, you can contact our support
					team directly through the "Report a Problem" feature. We have a dedicated team that will
					investigate and resolve disputes fairly based on the provided evidence and rules.
				</Accordion.Content>
			</Accordion.Item>
			<Accordion.Item value="item-9">
				<Accordion.Trigger>How can I improve my ranking on GamerFlux?</Accordion.Trigger>
				<Accordion.Content>
					Your ranking improves as you participate and perform well in tournaments. Winning games,
					advancing in brackets, and finishing in top positions will help you climb the leaderboard.
					You can also engage in regular practice matches or community events to boost your profile.
				</Accordion.Content>
			</Accordion.Item>
		</Accordion.Root>
	</div>
</div>
