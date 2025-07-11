<script lang="ts">
	// Types
	import type { PageProps } from "./$types";

	// Components
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import Pricing from "$lib/components/layout/Pricing.svelte";

	// Props
	const { data }: PageProps = $props();
</script>

<Pricing />

<Testimonials
	testimonials={[
		{
			name: "Keandra Williams",
			position: "VP of Business Development",
			company: "DataFlow Technologies",
			quote:
				"Suna saved us 18 hours weekly on prospect research. The autonomous LinkedIn and Crunchbase integration delivers qualified leads with zero manual work. ROI paid for itself in the first month.",
			image:
				"/generated/image-a-confident-african-american-business-wo.webp"
		},
		{
			name: "Marcus Chen",
			position: "Growth Operations Manager",
			company: "ScaleUp Solutions",
			quote:
				"The human approval workflow gives us confidence in AI decisions while maintaining speed. Open source transparency lets us audit exactly what Suna does with our data. Game-changer for our team.",
			image:
				"/generated/image-an-asian-american-male-business-developm.webp"
		},
		{
			name: "Isabella Rodriguez",
			position: "Head of Sales Operations",
			company: "Venture Dynamics",
			quote:
				"Multi-step workflow execution across platforms like we've never seen. Suna handles competitor analysis, lead scoring, and report generation in one autonomous sequence. Worth every credit.",
			image:
				"/generated/image-a-hispanic-female-entrepreneur-in-a-cont.webp"
		}
	]}
/>

<CallToAction
	title="Let your AI employee take it from here"
	subtitle="Stop wasting 15+ hours on research every week"
	description="Business development teams lose valuable time to repetitive tasks. Suna handles multi-step lead research, data extraction, and analysis—fully autonomously—with built-in human approvals when stakes are high. You stay in control while getting work off your plate."
	imageSrc="/generated/image-a-professional-business-person-smiling-w.webp"
	callsToAction={[
		{
			href: "/signup",
			label: "Get started free",
			variant: "primary"
		},
		{
			href: "/demo",
			label: "See what Suna can do",
			variant: "secondary"
		}
	]}
/>
