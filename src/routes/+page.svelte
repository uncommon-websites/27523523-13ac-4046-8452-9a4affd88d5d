<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CustomerCardHero from "$lib/components/layout/hero-sections/CustomerCardHero.svelte";

	// Icons
	import IconTrendingDown from "~icons/lucide/trending-down";
	import IconRefreshCw from "~icons/lucide/refresh-cw";
	import IconCloud from "~icons/lucide/cloud";
	import IconActivity from "~icons/lucide/activity";
	import IconCpu from "~icons/lucide/cpu";
	import IconZap from "~icons/lucide/zap";
</script>

<CustomerCardHero
	centered={true}
	title="80% cheaper AI training through automatic cross-cloud arbitrage"
	subtitle="Run your GPU workloads across AWS, GCP, Azure, and specialty providers with automatic spot instance orchestration. No more hunting for availability or managing preemptions."
	customers={[
		{
			name: "Dr. Maya Chen",
			position: "ML Research Lead",
			imageSrc: "/generated/image-professional-headshot-of-a-confident-fem.webp"
		},
		{
			name: "Alex Rodriguez",
			position: "AI Infrastructure Engineer",
			imageSrc: "/generated/image-professional-headshot-of-a-smiling-male-.webp"
		},
		{
			name: "Jordan Kim",
			position: "Senior ML Engineer",
			imageSrc: "/generated/image-professional-headshot-of-a-diverse-tech-.webp"
		}
	]}
	callsToAction={[
		{ href: "https://cloud.sf-tensor.com", label: "Join waitlist" },
		{ href: "mailto:collab@sf-tensor.com", label: "Talk to an engineer" }
	]}
/>
<LogoScroller
	label="Trusted by ML teams worldwide"
	logoUrls={[
		'https://cdn.brandfetch.io/huggingface.co/w/400/h/400/logo',
		'https://cdn.brandfetch.io/stability.ai/w/400/h/400/logo',
		'https://cdn.brandfetch.io/anthropic.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/cohere.com/w/400/h/400/logo'
	]}
/>

<Summary
	title="What we do"
	text="SF Tensor eliminates the complexity of running AI workloads across multiple cloud providers. We automatically find the cheapest available GPU compute across AWS, GCP, Azure, and specialty providers, then handle all the orchestration, migrations, and preemptions so ML engineers can focus on training models instead of managing infrastructure. It's cloud computing the way it was supposed to work: simple, affordable, and reliable."
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
<AboutTeaser generating />
<CallToAction generating />
