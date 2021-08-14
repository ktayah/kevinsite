<script>
	import Navbar from './components/Navbar.svelte';
</script>

<main>
	<div class="columns is-desktop">
		<div class="column">
			<Navbar />
		</div>
		<div class="column is-hidden-touch">
			<h1 class="title">
				Hello World
			  </h1>
			  <p class="subtitle">
				My first website with <strong>Bulma</strong>!
			  </p> 
		</div>
	</div>
</main>

<style lang="scss">
  @import './assets/styles/global.scss';

	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	.header-container {
		display: flex;
		flex-direction: row;
		flex: 1;
		height: 30rem;
		background-color: $background;

		.inner-header-container {
			display: flex;
			flex: 1;
			justify-content: center;
			align-items: center;
			flex-direction: column;
		}
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>