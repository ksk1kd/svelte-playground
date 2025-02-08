<script lang="ts">
import ComponentProps from './components/ComponentProps.svelte'
import ControlFlow from './components/ControlFlow.svelte'
import Derived from './components/Derived.svelte'
import Effect from './components/Effect.svelte'
import FormInputBinding from './components/FormInputBinding.svelte'
import Snippet from './components/Snippet.svelte'
</script>

<main>
  <div class="container">
    <Snippet />
    <Derived />
    <Effect />
    <ControlFlow />
    <ComponentProps />
    <FormInputBinding />
  </div>
</main>

<style>
.container {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
}
</style>
