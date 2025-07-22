<script lang="ts">
	import '../app.css';
	
	let { children } = $props();
</script>

<nav>
	<ul class="container mx-auto flex gap-4">
		<li><a href="/">Home</a></li>
		<li><a href="/search">All Resources</a></li>
	</ul>
</nav>

{@render children()}
