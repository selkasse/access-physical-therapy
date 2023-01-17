<script>
  import * as prismicH from "@prismicio/helpers";
  export let slice;
  const imageSrc = prismicH.asImageWidthSrcSet(slice.primary.main_image_file);
</script>

<!-- <div> -->
<div class="layout">
  <img
    src={imageSrc.src}
    srcset={imageSrc.srcset}
    alt={slice.primary.main_image_file.alt}
  />
</div>
