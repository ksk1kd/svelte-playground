<script lang="ts">
import { getContext } from 'svelte'

interface Counter {
  count: number
}

const value: Counter = getContext('counter')
</script>

<p>count: {value.count}</p>