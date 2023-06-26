<script lang="ts">
	import { page } from '$app/stores'
	import Item from '$lib/components/Navigation/item.svelte'

	//
</script>

<nav class=" p-4 flex justify-between flex-col h-full">
	<div class="space-y-4">
		<a href="/dashboard" class="text-center h4 hover:text-surface-900-50-token btn w-full">
			SubFlix App
		</a>
		<ul class="space-y-2">
			<li>
				<Item />
			</li>
			<li>
				<Item />
			</li>
		</ul>
	</div>
	<ul class="">
		{#if $page.url.pathname === `/group/create`}
			<li>
				<button
					type="button"
					class="btn variant-filled-error w-full"
					on:click={() => {
						window.history.back()
					}}
				>
					Back
				</button>
			</li>
		{:else}
			<li>
				<a href="/group/create" class="btn variant-filled-primary w-full"> Create </a>
			</li>
		{/if}
	</ul>
</nav>
