<script>
  import * as prismicH from "@prismicio/helpers";
  export let slice;
</script>

<div class="layout">
  <!-- {JSON.stringify(slice.items)} -->
  {#each slice.items as blurb}
    <!-- {JSON.stringify(blurb)} -->
    {@html prismicH.asHTML(blurb.blurb_rich_text)}
  {/each}
</div>

<!-- <pre>{JSON.stringify(slice, null, 2)}</pre> -->
