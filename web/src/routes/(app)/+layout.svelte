<script>
	import Navigation from '$lib/components/Navigation/Navigation.svelte'
	import { AppShell, Drawer } from '@skeletonlabs/skeleton'
</script>

<Drawer>(contents)</Drawer>

<AppShell slotSidebarLeft="bg-surface-600/10 shadow  w-0 lg:w-80">
	<svelte:fragment slot="sidebarLeft">
		<Navigation />
	</svelte:fragment>
	<div class="mx-auto p-4 space-y-4 h-full">
		<slot />
	</div>
</AppShell>
