<script lang="ts">
interface Props {
  string: string
  number: number
  boolean: boolean
  array: string[]
  optional?: string
}

let props: Props = $props()
</script>

<p>stringProp: {props.string}</p>
<p>numberProp: {props.number}</p>
<p>booleanProps: {props.boolean ? 'TRUE' : 'FALSE'}</p>
<p>arrayProps: {props.array}</p>