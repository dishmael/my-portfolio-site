<script lang="ts">
	import { writable } from 'svelte/store';

	let { title, href } = $props();
	const active = writable(false);

	$effect(() => {
		const targetSection = document.querySelector(href);
		if (!targetSection) return;

		const observer = new IntersectionObserver(
			(entries) => {
				entries.forEach((entry) => {
					active.set(entry.isIntersecting);
				});
			},
			{ threshold: 0.32 }
		);

		observer.observe(targetSection);

		return () => observer.unobserve(targetSection);
	});
</script>

<li>
  <a class="group flex items-center py-3 nav-link" href="{href}" class:active={$active}>
    <span class="nav-indicator mr-4 h-px"></span>
    <span class="nav-text text-xs font-bold tracking-widest uppercase">{title}</span>
  </a>
</li>

<style>
	.nav-link.active .nav-indicator {
		width: 72px;
		background-color: #e2e8f0;
	}

	.nav-link .nav-indicator {
		width: 32px;
		background-color: #64748b;
		transition:
			width 0.3s ease-in-out,
			background-color 0.3s ease-in-out;
	}

	.nav-link:hover .nav-indicator {
		width: 72px;
		background-color: #e2e8f0;
	}

	.nav-link.active .nav-text {
		color: #e2e8f0;
	}
</style>
