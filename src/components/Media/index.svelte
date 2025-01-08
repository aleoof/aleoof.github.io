<script>
	import './style.css';
	import Email from '../svg/Email.svelte';
	import Github from '../svg/Github.svelte';
	import Linkedin from '../svg/linkedin.svelte';
	let socialList = [
		{ id: 'linkedin', link: 'https://www.linkedin.com/in/alexandre-oof' },
		{ id: 'email', link: 'mailto:aleoof80@gmail.com' },
		{ id: 'github', link: 'https://github.com/aleoof' },
	];
</script>

<div class="media">
	{#each socialList as social}
		<a
			href={social.link}
			target="_blank"
			class="neon-svg"
			aria-label={social.id}
		>
			{#if social.id === 'linkedin'}
				<Linkedin />
			{:else if social.id === 'email'}
				<Email />
			{:else if social.id === 'github'}
				<Github />
			{/if}
		</a>
	{/each}
</div>
