<script>
	import notes from './data/index.json';

	const { classification, essentials, terminology } = notes;

	const typography = terminology.filter((word) => word.term === 'typography');
	// $: console.log(notes);
</script>

<main>
	<h1>Basic Typography Note</h1>
	<article>
		<dl>
			{#each typography as typography}
				<dt><b>{typography.term}</b></dt>
				<dd>- {typography.definition}</dd>
				<dd>- {typography.additional_info}</dd>
			{/each}
		</dl>
	</article>

	<section>
		<h2>Terminology</h2>
		<h3>The Anatomy of a Typeface</h3>
		<dl>
			{#each terminology as terminology}
				{#if terminology.term !== 'typography'}
					<dt><b>{terminology.term}</b></dt>
					<dd>- {terminology.definition}</dd>

					{#if terminology.additional_info}
						<dd>*{terminology.additional_info}</dd>
					{/if}
				{/if}
			{/each}
		</dl>
	</section>

	<section>
		<h3>Common Font Classification Types</h3>
		<dl>
			{#each classification as classification}
				<dt><b>{classification.term}</b></dt>
				<dd>- {classification.definition}</dd>

				{#if classification.additional_info}
					<dd>*{classification.additional_info}</dd>
				{/if}
			{/each}
		</dl>
	</section>

	<section>
		<h2>Typography Essentials</h2>
		<dl>
			{#each essentials as essentials}
				<dt><b>{essentials.term}</b></dt>
				<dd>- {essentials.definition}</dd>

				{#if essentials.additional_info}
					<dd>*{essentials.additional_info}</dd>
				{/if}
			{/each}
		</dl>
	</section>

	<!-- <h2>Typography Code Basics Essentials</h2> -->
	<!-- <h2>Source</h2> -->
</main>

<style>
	/*  */
</style>
