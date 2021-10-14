<script lang="ts">
  export let linkUrl: string;
  export let imageUrl: string;
  export let imageDescription: string;
  export let title: string;
  export let metadata: string;
</script>

<section class="mzp-c-card mzp-c-card-extra-small has-aspect-3-2">
  <a class="mzp-c-card-block-link" href={linkUrl}>
    <div class="mzp-c-card-media-wrapper">
      <img class="mzp-c-card-image" src={imageUrl} alt={imageDescription}/>
    </div>
    <div class="mzp-c-card-content">
      <h2 class="mzp-c-card-title">{title}</h2>
      <p class="mzp-c-card-meta">{metadata}</p>
    </div>
  </a>
</section>