<script lang="ts">
	import type { EnhancedImgAttributes } from '@sveltejs/enhanced-img';

	const {
		class: className,
		src,
		alt = '',
		loading = 'lazy',
		fetchpriority = 'auto'
	}: EnhancedImgAttributes = $props();
</script>

<enhanced:img
	class={className}
	src={src || ''}
	{alt}
	sizes="min(1280px, 100vw)"
	{loading}
	{fetchpriority}
/>
