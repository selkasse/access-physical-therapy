<script>
  import * as prismicH from "@prismicio/helpers";
  export let slice;
</script>

<div class="layout">
  {#each slice.items as blurb}
    <article>
      {@html prismicH.asHTML(blurb.blurb_rich_text)}
    </article>
  {/each}
</div>

<!-- <pre>{JSON.stringify(slice, null, 2)}</pre> -->
