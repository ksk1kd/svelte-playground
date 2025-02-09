<script lang="ts">
import Bindable from './components/Bindable.svelte'
import ComponentProps from './components/ComponentProps.svelte'
import ContextCounterControls from './components/ContextCounterControls.svelte'
import ContextCounterDisplay from './components/ContextCounterDisplay.svelte'
import ContextCounterProvider from './components/ContextCounterProvider.svelte'
import ControlFlow from './components/ControlFlow.svelte'
import Derived from './components/Derived.svelte'
import Effect from './components/Effect.svelte'
import FormInputBinding from './components/FormInputBinding.svelte'
import Snippet from './components/Snippet.svelte'
</script>

<main>
  <div class="container">
    <ContextCounterProvider />
    <Bindable />
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
