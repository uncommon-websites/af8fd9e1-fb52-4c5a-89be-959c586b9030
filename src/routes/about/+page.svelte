<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Icons
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Heritage craftsmanship",
			description: "Four decades of family tradition, where master artisans transform premium leather into generational heirlooms using time-honored techniques."
		},
		{
			title: "Sustainable beauty",
			description: "Creating lasting pieces that replace disposable fashion, reducing waste while celebrating the natural elegance of ethically-sourced materials."
		},
		{
			title: "Artisan authenticity",
			description: "Every piece tells a story of skilled hands and patient craft, honoring traditional methods while embracing modern bohemian spirit."
		}
	];
</script>

<SecondaryHero
	title="Solving world hunger"
	subtitle="one step at a time"
	imageSrc="https://www.unc.mn/image-placeholder.svg"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"We started in 2018 with a simple goal: make helpful tech that people actually need. While many chase profits, we chose to do things differently.",
		"Beyond making good products, we care about doing the right thing, being kind to our planet, and making sure everyone can use what we build. That's our compass.",
		"From day one, we've asked ourselves: 'Does this actually help people?' This question gets us through tough calls and shapes who we are. We're playing the long game here.",
		"We think about how our work affects real people's lives. We build tech that brings people together, keeps your information safe, and treats everyone fairly. When we stick to these basics, good things happen."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- CTA Section -->
<CallToAction
	title="Discover your perfect piece"
	subtitle="Crafted for the conscious woman"
	description="Experience leather accessories that honor both tradition and your unique style. Each piece is thoughtfully designed to become a cherished part of your journey, from everyday adventures to life's most meaningful moments."
/>
