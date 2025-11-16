<script lang="ts">
  import '@sakun/system.css';
  import "../app.css"
  let { children } = $props();
</script>

<svelte:head>
</svelte:head>

{@render children()}
