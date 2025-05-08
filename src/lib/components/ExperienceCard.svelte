<script lang="ts">
	let { heading, from, to, skills = [], children } = $props();
</script>

<li class="mb-12">
	<div
		class="group relative grid pb-1 transition-all sm:grid-cols-8 sm:gap-8 md:gap-4 lg:group-hover/list:opacity-50 lg:hover:!opacity-100"
	>
		<div
			class="absolute -inset-x-4 -inset-y-4 z-0 hidden rounded-md transition motion-reduce:transition-none lg:-inset-x-6 lg:block lg:group-hover:bg-slate-800/50 lg:group-hover:shadow-[inset_0_1px_0_0_rgba(148,163,184,0.1)] lg:group-hover:drop-shadow-lg"
		></div>
		<header
			class="z-10 mt-1 mb-2 text-xs font-semibold tracking-wide text-slate-500 uppercase sm:col-span-2"
			aria-label="2024 to Present"
		>
			{from} — {to}
		</header>
		<div class="z-10 sm:col-span-6">
			<h3 class="leading-snug font-medium text-slate-200">
				<div>{heading}</div>
			</h3>
			{#if children}
				<div class="mt-2 text-sm text-slate-400">{@render children()}</div>
			{/if}
			<ul class="mt-2 flex flex-wrap" aria-label="Technologies used">
				{#each skills as skill}
					<li class="mt-2 mr-1.5">
						<div
							class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs leading-5 font-medium text-teal-300"
						>
							{skill}
						</div>
					</li>
				{/each}
			</ul>
		</div>
	</div>
</li>

<style></style>
