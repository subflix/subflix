<script>
	import Navigation from '$lib/components/Navigation/Navigation.svelte'
	import { AppBar, AppShell, Drawer } from '@skeletonlabs/skeleton'
</script>

<Drawer>(contents)</Drawer>

<AppShell slotSidebarLeft="bg-surface-600/10 shadow  w-0 lg:w-64">
	<svelte:fragment slot="header">
		<AppBar background="bg-surface-600/10" shadow="shadow-sm">
			<svelte:fragment slot="lead">
				<div class="flex items-center">
					<button class="lg:hidden btn btn-sm mr-4">
						<span>
							<svg viewBox="0 0 100 80" class="fill-token w-4 h-4">
								<rect width="100" height="20" />
								<rect y="30" width="100" height="20" />
								<rect y="60" width="100" height="20" />
							</svg>
						</span>
					</button>
					<strong class="text-xl uppercase">Skeleton</strong>
				</div>
			</svelte:fragment>
		</AppBar>
	</svelte:fragment>
	<svelte:fragment slot="sidebarLeft">
		<Navigation />
	</svelte:fragment>

	<slot />
	<svelte:fragment slot="pageFooter">Page Footer</svelte:fragment>
</AppShell>
