<script lang="ts">
let { value = $bindable() } = $props()
</script>

<input bind:value={value} />