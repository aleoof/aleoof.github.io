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
<div class="content">
<div class="container" >
  <div class="copy">
    <h2 class="subtitle neon">Front End Developer</h2>
    <h1 class="title neon">Alexandre Oliveira</h1>
    <div class="media">
      {#each socialList as social}
      <a href={social.link} target="_blank" class="neon-svg">
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
    <div>
      <div class="frame">
        <img alt="developer" class="image-icon" height="250px" width="250px" src="https://media.licdn.com/dms/image/v2/D4D03AQHBxQ2Zc7S5kA/profile-displayphoto-shrink_800_800/profile-displayphoto-shrink_800_800/0/1724951884339?e=1741219200&v=beta&t=sfwvnB23pvAp93JQ7DUKdbcKof9oj-BKzs9dok1nhrQ"/>
      </div>
    </div>
  </div>
</div>