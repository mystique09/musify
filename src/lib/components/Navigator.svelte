<script>
  export let heading;
  export let list;
  export let url;
</script>

<div class="navigator">
  <th>{heading}</th>
  {#each list as link}
    <td><a href={url}>{link}</a></td>
  {/each}
</div>
<style>
  .navigator {
    @apply flex flex-col py-4;
  }
  
  th {
    @apply text-left text-gray-400 font-bold text-sm uppercase;
  }
  td {
    @apply text-white text-sm font-medium mt-4;
  }
</style>