<script lang="ts">
	import '../../app.css';
	import { onMount } from 'svelte';

  	onMount(() => { /* picks random intro subtext, typescript gets a little mad */
		(function introPick() {
			var intros = ['Getting bored is lame', 'Made with love', 'Sometimes they work', 'HELLO EMPLOYERS', 'Wanna see a magic trick?', ':3'];
			var randomFact = Math.floor(Math.random() * intros.length);
			document.getElementById('introDisplay')!.innerHTML = intros[randomFact];
		})();
	})
</script>

<div class="project-welcome">
	<h1>Projects Collection</h1>
	<p id="introDisplay"></p>
</div>
