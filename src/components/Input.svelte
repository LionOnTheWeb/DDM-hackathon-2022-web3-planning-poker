<script>
export let label = ""
export let type = ""
export let placeholder = null

</script>

{#if label}
  <label>{label}</label>
{/if}

<input class="test" type="{type}" placeholder="{placeholder}" />