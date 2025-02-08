<script lang="ts">

</script>

<h1>Snippet</h1>

{#snippet hello(name: string)}
  <p>Hello {name}</p>
{/snippet}

{@render hello('bob')}
{@render hello('alice')}
{@render hello('charlie')}