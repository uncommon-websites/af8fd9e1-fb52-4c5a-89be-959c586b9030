<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";
</script>

<Hero
	title="Crafted to last. Made to be passed."
	subtitle="Timeless leather bags handmade by artisans."
	imageSrc="/generated/image-a-sophisticated-woman-with-a-bohemian-st.webp"
	centered={false}
/>
<LogoScroller
	label="Trusted by fashion-forward professionals"
	logoUrls={[
		'https://cdn.brandfetch.io/anthropologie.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/nordstrom.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/freepeople.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/modcloth.com/w/400/h/400/logo'
	]}
/>

<Summary
	generating
	title="What we do"
	text="Our technology delivers measurable results through secure, adaptable solutions that directly increase productivity and drive growth."
/>

<Testimonials
	generating
	testimonials={[
		{
			name: "Jane Smith",
			position: "CTO",
			company: "Tech Innovations",
			quote:
				"Their cutting-edge automation boosted our productivity by 35%.\nThe intuitive interface reduced training time and improved team adoption.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "John Doe",
			position: "Director of Operations",
			company: "Global Solutions",
			quote:
				"Their robust security protocols gave us confidence in handling sensitive data.\nThe 24/7 support team resolved issues within hours, not days.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Sarah Johnson",
			position: "Product Manager",
			company: "Future Systems",
			quote:
				"The scalable platform grew seamlessly with our business needs.\nTheir customization options allowed us to tailor solutions perfectly to our workflows.",
			image: "https://www.unc.mn/image-placeholder.svg"
		}
	]}
/>

<Features
	generating
	title="Features"
	subtitle="Some features"
	features={[
		{
			title: "Streamlined Workflows",
			description:
				"Automate repetitive tasks and connect systems to improve productivity with our industry-leading 87% time savings."
		},
		{
			title: "Data Analysis",
			description:
				"Extract meaningful insights from your data with powerful analytical tools backed by proprietary AI algorithms that are 3x more accurate than competitors."
		},
		{
			title: "Secure Collaboration",
			description:
				"Work together seamlessly while maintaining strict data privacy standards with our zero-knowledge architecture and military-grade encryption."
		}
	]}
/>
<AboutTeaser />
<CallToAction
	title="Ready for a bag that becomes part of your story?"
	subtitle="Step away from fast fashion"
	description="Our leather goods are crafted by hand, designed for self-expression, and made to last—so you can invest in style that stays with you for life. Four decades of family craftsmanship meets award-winning design."
	imageSrc="/generated/image-a-relaxed-confident-bohemian-woman-walki.webp"
	callsToAction={[
		{
			href: "/shop",
			label: "Shop the collection",
			variant: "primary"
		},
		{
			href: "/craftsmanship",
			label: "See our story",
			variant: "secondary"
		}
	]}
/>
