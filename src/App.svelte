<script>
	import Navbar from './components/Navbar.svelte';
	import Main from './components/Main.svelte';
	import About from './components/About.svelte';
	import Skills from './components/Skills.svelte';
	import Experience from './components/Experience.svelte';
	import Education from './components/Education.svelte';
	import Achievements from './components/Achievements.svelte';
	import Contact from './components/Contact.svelte';
	let me = 'static/images/me.png';
</script>

<main>
	<div class="columns is-desktop">
		<div class="column">
			<Navbar />
			<Main />
			<About />
			<Skills />
			<Experience />
			<Education />
			<Achievements />
			<Contact />
		</div>
	</div>
	<div id="fixed" class="column is-hidden-touch" >
		<img src={me} alt="me" id="image" />
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

	#fixed {
		position: fixed;
		bottom: 0;
		top: 0;
		right: 0;
		padding: 0;
	}

	#image {
		height: 100%;
		width: auto;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>