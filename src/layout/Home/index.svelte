<script lang="ts">
	import Github from './../../components/svg/Github.svelte';
	import Email from '../../components/svg/Email.svelte';
	import Linkedin from '../../components/svg/linkedin.svelte';
  import './style.css'
  let socialList = [
    { id: "linkedin" ,link:"https://www.linkedin.com/in/alexandre-oof"},
    { id:"email", link:"mailto:aleoof80@gmail.com"},
    { id:"github", link:"https://github.com/aleoof"},
    ]
</script>
<div class="container" >
  <h1 class="title">Alexandre Oliveira</h1>
  <h2 class="subtitle">Front End Developer</h2>
  <div class="media">
    {#each socialList as social}
      <a href={social.link} target="_blank">
      {#if social.id === "linkedin"}
          <Linkedin/>
        {:else if social.id === "email"}
          <Email/>
        {:else if social.id === "github"}
          <Github/>
        {/if}
      </a>
    {/each}
  </div>
</div>