<script lang="ts">
import { setContext } from 'svelte'
import ContextCounterControls from './ContextCounterControls.svelte'
import ContextCounterDisplay from './ContextCounterDisplay.svelte'

let value = $state({ count: 0 })
setContext('counter', value)
</script>

<h1>Context</h1>

<ContextCounterControls />
<ContextCounterDisplay />