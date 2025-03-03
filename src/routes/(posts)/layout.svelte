<script lang="ts">
  const props = $props();
  const children = props.children;

  console.log(props);
  const title = props.title ?? "Blog";
  const description = props.description ?? "A blog about stuff";
</script>

<svelte:head>
  <title>{title}</title>
  <meta name="description" content={description} />
</svelte:head>

{@render children()}
