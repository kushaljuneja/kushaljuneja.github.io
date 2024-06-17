<script lang="ts">
  import Seo from "$lib/components/Seo.svelte";
  import WritingList from "./BlogList.svelte";
  import writing from "./blog.yaml";

  export let posts = writing.posts !== null ? writing.posts : [];
</script>

<Seo title="Kushal Juneja – Blog" />

<section class="layout-md py-12">
  <div class="space-y-5">This is my personal blog. Here, I write about topics that feel like <em>spinning plates</em> to me. <em>Spinning plates</em> is a reference to one of the classic Richard Feynmann stories, in which Richard Feynmann rediscovers what it's like to enjoy physics by delighting playfully in seemingly-unimportant physics problems.</div>
  <div class="py-12">
  {#if posts.length === 0}
  <div class="space-y-5 font-bold">Work in Progress! Check back later.</div>
  {:else}
    <WritingList data={posts} />
  {/if}
  </div>
</section>
