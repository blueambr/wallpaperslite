<script lang="ts">
	import type { Icon as IconType } from '@lucide/svelte';

	const {
		class: className,
		i: Icon,
		size = 28
	} = $props<{ class?: string; i: typeof IconType; size?: number }>();
</script>

<Icon class={className} {size} strokeWidth={1.5} />
