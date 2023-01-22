<script>
  import * as prismicH from "@prismicio/helpers";
  export let slice;
</script>

<div class="layout freefloat" style="margin-top: 10px">
  {@html prismicH.asHTML(slice.primary.single_paragraph_text)}
</div>

<!-- <pre>{JSON.stringify(slice, null, 2)}</pre> -->
