<script lang="ts">
  import Instance from './Instance.svelte'

  const instancesData = [
    {
      linkUrl: "https://councildataproject.org/seattle",
      imageUrl: "static/imgs/seattle.jpg",
      imageDescription: "Seattle skyline",
      title: "City of Seattle, Washington",
      metadata: "Maintained by the CDP Core Team",
    },
  ];
</script>

<div id="instances" class="cdp-bg-light-grey">
  <div class="mzp-l-content mzp-t-content-xl">
    <h1 class="mzp-c-article-title">CDP Instances</h1>
    <p>All currently maintained Council Data Project instances.</p>
    {#each instancesData as instance}
      <div class="mzp-l-card-third">
        <Instance 
          linkUrl={instance.linkUrl}
          imageUrl={instance.imageUrl}
          imageDescription={instance.imageDescription}
          title={instance.title}
          metadata={instance.metadata}
        />
      </div>
    {/each}
  </div>
</div>