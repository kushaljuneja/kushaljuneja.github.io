<script lang="ts">
  import Seo from "$lib/components/Seo.svelte";
  import WritingList from "./BlogList.svelte";
  import writing from "./blog.yaml";
</script>

<Seo
  title="Kushal Juneja – Blog"
  description="Blog Posts"
/>

<section class="layout-md py-12">
  <WritingList data={writing.posts} />
</section>

