<script lang="ts">
	import './style.css';
	import Media from '../../components/Media/index.svelte';
	import Avatar from '../../components/Avatar/index.svelte';
</script>

<svelte:head>
	<title>Alexandre Oliveira</title>
	<meta
		name="description"
		content="Alexandre Oliveira Full Stack Web Developer "
	/>
</svelte:head>
<div class="content">
	<div class="container">
		<div class="copy">
			<h2 class="subtitle neon">
				<strong> Full Stack Developer</strong>
			</h2>
			<h1 class="title neon">Alexandre Oliveira</h1>
			<Media />
		</div>
		<div>
			<Avatar />
		</div>
	</div>
</div>
