<script lang="ts">
  const recents = [
    {
      title: 'Everyone makes decisions in their own interests',
      url: '/blog/everyone-makes-decisions-in-their-own-interests'
    }
  ]
</script>

<ul>
  {#each recents as { title, url }}
    <li>
      <a href={url}>
        {title}
      </a>
    </li>
  {/each}
</ul>
