<script lang="ts">
let condition = 18
</script>

<h1>Control Flow</h1>

<section>
  <h2>If</h2>
  {#if condition >= 20}
    <p>Adult</p>
  {:else if condition >= 0}
    <p>Child</p>
  {:else}
    <p>Invalid</p>
  {/if}
</section>

<section>
  <h2>Each</h2>
  {#each [1, 2, 3] as number}
    <p>{number}</p>
  {/each}
</section>