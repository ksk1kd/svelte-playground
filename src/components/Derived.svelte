<script lang="ts">
let count = $state(0)
let double = $derived(count * 2)
</script>

<h1>Derived</h1>

<button onclick={() => {count++}}>Increment</button>
<p>Count: {count}</p>
<p>Double: {double}</p>