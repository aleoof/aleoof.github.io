<script lang="ts">
	import Media from '../../components/Media/index.svelte';
	import Avatar from '../../components/Avatar/index.svelte';
	import Meta from '../../components/Meta/index.svelte';
	import Container from '../../components/Container/index.svelte';
</script>

<Meta />
<div class="content">
	<Container>
		<div class="copy">
			<h2 class="subtitle neon">Full Stack Developer</h2>
			<h1 class="title neon">Alexandre Oliveira</h1>
			<Media />
		</div>
		<div>
			<Avatar />
		</div>
	</Container>
</div>

<style>
	@import './style.css';
</style>
