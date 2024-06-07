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
  <h2 class="heading2">Notes and Tutorials</h2>
  <WritingList data={writing.notes} />
</section>

<section class="layout-md py-12">
  <h2 class="heading2">Academic Writing</h2>
  <WritingList data={writing.papers} />
</section>
