<script>
export let label = ""
export let type = ""
export let value = ""
export let placeholder = null

</script>

{#if label}
  <label>{label}</label>
{/if}

<input type="{type}" placeholder="{placeholder}" value="{value}"/>