<script lang="ts">
	interface Props {
		content: string;
	}

	const { content }: Props = $props();
</script>

<section>
	<div class="container max-w-3xl">
		<article class="prose max-w-none prose-blockquote:not-italic prose-invert prose-lg">
			{@html content}
		</article>
	</div>
</section>
