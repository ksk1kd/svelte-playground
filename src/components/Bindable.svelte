<script lang="ts">
import BindableChild from './BindableChild.svelte'
let input = $state('')
</script>

<h1>Bindable</h1>

<BindableChild bind:value={input} />
<p>input: {input}</p>