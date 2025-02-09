<script lang="ts">
import { getContext } from 'svelte'

interface Counter {
  count: number
}

const value: Counter = getContext('counter')
</script>
  
<button onclick={() => value.count++}>Increment</button>