<script lang="ts">
	import '../app.css';
	import { page } from '$app/stores';
</script>

<div class="header">
	<img width=69px src="../cherry2.svg" alt="logo" class="logo">
	<div class="header-right">
	  <a class:active={$page.url.pathname === ""} href="/">Home</a>
	  <a href="/posts">Projects</a>
	  <a href="/posts/create">Yapping</a>
	</div>
  </div> 

<slot />
