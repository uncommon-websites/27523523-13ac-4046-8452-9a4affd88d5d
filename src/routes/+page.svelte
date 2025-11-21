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
<<<<<<< HEAD
	text="SF Tensor eliminates the complexity of running AI workloads across multiple cloud providers. We automatically find the cheapest available GPU compute across AWS, GCP, Azure, and specialty providers, then handle all the orchestration, migrations, and preemptions so ML engineers can focus on training models instead of managing infrastructure. It's cloud computing the way it was supposed to work: simple, affordable, and reliable."
=======
	text="SF Tensor eliminates the complexity of multi-cloud GPU management for ML engineers at AI startups. We automatically orchestrate spot instances across AWS, GCP, Azure, and specialty providers, delivering up to 80% cost savings while handling preemptions and availability hunting for you. Focus on training models, not managing infrastructure."
>>>>>>> 92b8c6ea001ce2dfde9f714ca33e3c6b8e111e34
/>

<Testimonials
	testimonials={[
		{
			name: "Priya Rajagopalan",
			position: "ML Engineer",
			company: "Anthropic",
			quote:
				"We cut our training costs by 73% in the first month. The automatic spot instance migration means our experiments never fail halfway through, and we stopped worrying about which cloud provider has H100s available.",
			image: "/generated/image-environmental-portrait-of-a-south-asian-.webp"
		},
		{
			name: "Marcus Chen",
			position: "Head of AI Infrastructure",
			company: "Stability AI",
			quote:
				"Before SF Tensor, we had two engineers just managing cloud providers and babysitting spot instances. Now that's automated and they're building features. The ROI was immediate.",
			image: "/generated/image-thoughtful-environmental-headshot-of-an-.webp"
		},
		{
			name: "Amara Okonkwo",
			position: "Research Lead",
			company: "Cohere",
			quote:
				"The cross-cloud arbitrage is genuinely magical. We kick off a training run and SF Tensor finds the cheapest compute across all providers in real-time. No preemption headaches, no availability hunting.",
			image: "/generated/image-warm-confident-environmental-portrait-of.webp"
		}
	]}
/>

<Features
	title="Built for the reality of multi-cloud GPU infrastructure"
	subtitle="Stop wrestling with cloud complexity and start training faster"
	features={[
		{
			title: "80% cost reduction through intelligent arbitrage",
			description:
				"Automatically find and orchestrate the cheapest GPU compute across AWS, GCP, Azure, and specialty providers in real-time."
		},
		{
			title: "Zero-downtime spot instance migration",
			description:
				"Your training jobs survive preemptions with automatic checkpoint and migration—no manual intervention, no lost progress."
		},
		{
			title: "Hardware-agnostic compute platform",
			description:
				"Run on H100s, A100s, TPUs, or Trainium without rewriting code. Your workloads adapt automatically to available hardware."
		},
		{
			title: "Real-time price intelligence",
			description:
				"Track GPU pricing across every provider every few minutes and automatically shift workloads to capture savings."
		},
		{
			title: "One interface for all clouds",
			description:
				"Deploy across multiple providers without managing separate AWS, GCP, and Azure configurations. Use your existing credits or pay through us."
		},
		{
			title: "Automatic kernel optimization",
			description:
				"Transform training kernels into mathematically optimal forms by simulating memory, cache, and hardware topology for maximum performance."
		}
	]}
/>
<AboutTeaser />
<CallToAction 
	title="Stop overpaying for GPU compute"
	subtitle="Join the waitlist today"
	description="ML teams are cutting training costs by up to 80% with SF Tensor's automatic cross-cloud orchestration. No more hunting for availability, no preemption headaches, no cloud complexity. Just faster, cheaper training runs that actually complete."
	imageSrc="/generated/image-a-mid-30s-ml-engineer-sits-at-a-modern-d.webp"
	callsToAction={[
		{ href: "https://cloud.sf-tensor.com", label: "Join waitlist", variant: "primary" },
		{ href: "mailto:collab@sf-tensor.com", label: "Talk to an engineer", variant: "secondary" }
	]}
/>
