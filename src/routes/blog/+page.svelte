<script lang="ts">
  import Seo from "$lib/components/Seo.svelte";
  import WritingList from "./BlogList.svelte";
  import writing from "./blog.yaml";

  export let posts = writing.posts !== null ? writing.posts : [];
</script>

<Seo
  title="Kushal Juneja – Blog"
/>

<section class="layout-md py-12">
  {#if posts.length === 0}
  <div class="layout-md text-lg space-y-14">
    Work in Progress!
  </div>
  {:else}
    <WritingList data={posts} />
  {/if}
  
</section>

