<script lang="ts">
const options = ['option1', 'option2', 'option3']
let text = $state('')
let checked = $state(false)
let radio = $state(options[0])
let select = $state(options[0])
let checkboxes = $state([])
</script>

<h1>Form Input Binding</h1>

<section>
  <h2>Text</h2>
  <input bind:value={text} />
  <p>Text: {text}</p>
</section>

<section>
  <h2>Checkbox</h2>
  <input type="checkbox" bind:checked={checked} />
  <p>Checkbox: {checked ? 'TRUE' : 'FALSE'}</p>
</section>

<section>
  <h2>Radio</h2>
  {#each options as option}
    <label>
      <input
        type="radio"
        bind:group={radio}
        value={option}
      />
      {option}
    </label>
  {/each}
  <p>Radio: {radio}</p>
</section>

<section>
  <h2>Select</h2>
  <select bind:value={select}>
    {#each options as option}
      <option value={option}>{option}</option>
    {/each}
  </select>
  <p>Select: {select}</p>
</section>

<section>
  <h2>Multiple Checkbox</h2>
  {#each options as option}
    <label>
      <input
        type="checkbox"
        bind:group={checkboxes}
        value={option}
      />
      {option}
    </label>
  {/each}
  <p>Multiple Checkbox: {checkboxes.join(', ')}</p>
</section>