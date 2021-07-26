<script>
	import notes from './data/index.json';

	const { classification, essentials, terminology } = notes;

	const typography = terminology.filter((word) => word.term === 'typography');
	// $: console.log(typography);
</script>

<main>
	<h1>Basic Typography Note</h1>
	<dl>
		{#each typography as typography}
			<dt>{typography.term}</dt>
			<dd>- {typography.definition}</dd>
			<dd>- {typography.additional_info}</dd>
		{/each}
	</dl>

	<h2>Terminology</h2>
	<h3>The Anatomy of a Typeface</h3>
	<dl>
		{#each terminology as terminology}
			{#if terminology.term !== 'typography'}
				<dt>{terminology.term}</dt>
				<dd>- {terminology.definition}</dd>

				{#if terminology.additional_info}
					<dd>- {terminology.additional_info}</dd>
				{/if}
			{/if}
		{/each}
	</dl>
</main>

<style>
	/*  */
</style>
