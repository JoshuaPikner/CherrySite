<script lang="ts">
	import '../../app.css';
	import { onMount } from 'svelte';

	onMount(() => {
		/* picks random intro subtext, typescript gets a little mad without the onMount for god knows why */
		(function introPick() {
			var intros = [
				'Getting bored is lame',
				'Made with love',
				'Sometimes they work',
				'HELLO EMPLOYERS',
				'Wanna see a magic trick?',
				':3'
			];
			var randomFact = Math.floor(Math.random() * intros.length);
			document.getElementById('introDisplay')!.innerHTML = intros[randomFact];
		})();
	});
</script>

<div class="project-welcome">
	<h1>Projects Collection</h1>
	<p id="introDisplay"></p>
</div>

<div class="container">
	<div class="single">
		<img src="https://picsum.photos/292/150" alt="lorem picsum" />
		<p>nerd emoji</p>
	</div>
	<div class="single">
		<img src="https://picsum.photos/292/150" alt="lorem picsum" />
		<p>good heavens</p>
	</div>
	<div class="single">
		<img src="https://picsum.photos/292/150" alt="lorem picsum" />
		<p>good heavens</p>
	</div>
	<div class="single">
		<img src="https://picsum.photos/292/150" alt="lorem picsum" />
		<p>good heavens</p>
	</div>
	<div class="single">
		<img src="https://picsum.photos/292/150" alt="lorem picsum" />
		<p>good heavens</p>
	</div>
	<div class="single">
		<img src="https://picsum.photos/292/150" alt="lorem picsum" />
		<p>good heavens</p>
	</div>
	<div class="single">
		<img src="https://picsum.photos/292/150" alt="lorem picsum" />
		<p>good heavens</p>
	</div>
	<div class="single">
		<img src="https://picsum.photos/292/150" alt="lorem picsum" />
		<p>good heavens</p>
	</div>
</div>
