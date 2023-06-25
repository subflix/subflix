<script>
	import { AppShell } from '@skeletonlabs/skeleton'
</script>

<AppShell>
	<svelte:fragment slot="header">Header</svelte:fragment>
	<div class="container mx-auto">
		<slot />
	</div>
	<svelte:fragment slot="pageFooter">Page Footer</svelte:fragment>
</AppShell>
