<!--
@component AboutTeaser
A minimalist teaser for the about page.
-->
<script lang="ts">
	// Types
	type TeamMember = {
		name: string;
		role: string;
		image: string;
	};

	// Components
	import Button from "../ui/Button.svelte";
	import ScrollText from "./sub/ScrollText.svelte";

	// State
	let sectionRef: HTMLElement;

	let props = $props();

	// Data
	const teamMember: TeamMember = {
		name: "Isabella Cruz",
		role: "Founder & Master Artisan",
		image: "/generated/image-a-female-artisan-founder-working-in-a-su.webp"
	};
</script>

<section bind:this={sectionRef} {...props}>
	<div class="section-px section-py container mx-auto">
		<div class="relative mx-auto grid max-w-2xl place-items-center gap-16">
			<ScrollText
				class="text-title1 text-center"
				text={`"I grew up in my parents' workshop, where every bag started with a story and ended in someone's hands for life. After watching fast fashion erase so much meaning, I set out to revive our family's craft—creating leather goods that honor the past and are worthy of the next generation."`}
			/>

			<!-- Team Member & CTA Section -->
			<div class="grid items-center gap-8 dark:border-gray-800">
				<div class="flex items-center justify-start gap-4">
					<img
						src={teamMember.image}
						alt={teamMember.name}
						class="size-12 rounded-full object-cover"
					/>
					<div>
						<div class="text-callout">{teamMember.name}</div>
						<div class="text-caption text-emphasis-low">{teamMember.role}</div>
					</div>
					<Button href="/about" variant="secondary" size="sm" class="ml-8">Read more</Button>
				</div>
			</div>
		</div>
	</div>
</section>
