<script lang="ts">
let count = $state(0)
$effect(() => {
  console.log(count)
})
</script>

<h1>Effect</h1>

<button onclick={() => {count++}}>Increment</button>