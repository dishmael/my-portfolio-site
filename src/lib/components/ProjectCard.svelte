<script lang="ts">
	let { heading, imgSrc, skills = [], children } = $props();
</script>

<div
	class="group relative grid gap-4 mt-8 pb-1 transition-all sm:grid-cols-8 sm:gap-8 md:gap-4 lg:group-hover/list:opacity-50 lg:hover:!opacity-100"
>
	<div
		class="absolute -inset-x-4 -inset-y-4 z-0 hidden rounded-md transition motion-reduce:transition-none lg:-inset-x-6 lg:block lg:group-hover:bg-slate-800/50 lg:group-hover:shadow-[inset_0_1px_0_0_rgba(148,163,184,0.1)] lg:group-hover:drop-shadow-lg"
	></div>
	<div class="z-10 sm:order-2 sm:col-span-6">
		<h3 class="font-bold">{heading}</h3>
		{#if children}
			<div class="mt-2 text-sm text-slate-400">{@render children()}</div>
		{/if}
		<ul class="mt-2 flex flex-wrap" aria-label="Technologies used:">
			{#each skills as skill}
				<li class="mt-2 mr-1.5">
					<div
						class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs leading-5 font-light text-teal-300"
					>
						{skill}
					</div>
				</li>
			{/each}
		</ul>
	</div>
	<img
		alt={heading}
		loading="lazy"
		width="200"
		height="48"
		decoding="async"
		data-nimg="1"
		class="aspect-video rounded border-2 border-slate-200/10 object-cover transition group-hover:border-slate-200/30 sm:order-1 sm:col-span-2 sm:translate-y-1"
		style="color:transparent"
		srcset=""
		src={imgSrc}
	/>
</div>

<style></style>
