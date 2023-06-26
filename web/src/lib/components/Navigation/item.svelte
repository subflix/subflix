<script lang="ts">
	export let id = 1
	export let name = 'group.name'
	export let members = [
		{
			id: 1,
			name: 'firstname lastname'
		}
	]

	$: console.log(members)
</script>

<a
	href="/group/{id}"
	class="p-2.5 rounded border border-primary-500 grid grid-cols-1 hover:bg-surface-300/50"
>
	<div>
		<p class="font-semibold">{name}</p>
	</div>
	<div class="">
		<span class="text-surface-900"> asd </span>
	</div>
</a>
