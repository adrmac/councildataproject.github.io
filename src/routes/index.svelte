<script lang="ts">
  import '@mozilla-protocol/core/protocol/css/protocol.css';
  import '@mozilla-protocol/core/protocol/css/protocol-components.css';
  import '@councildataproject/cdp-design/dist/colors.css';
  import '@councildataproject/cdp-design/dist/images.css';
  import '@councildataproject/cdp-design/dist/text.css';

  import NavBar from '../components/NavBar.svelte';
  import Hero from '../components/Hero.svelte';
  import SplitContainer from '../components/experiments/SplitContainer.svelte';
  import SplitContainerDark from '../components/experiments/SplitContainerDark.svelte';
  import CallOut from '../components/experiments/CallOut.svelte';
  import EmphasisBox from '../components/experiments/EmphasisBox.svelte';
  import About from '../components/old-website/About.svelte';
  import Instances from '../components/old-website/Instances.svelte';
  import Contributing from '../components/old-website/Contributing.svelte';
  import Footer from '../components/Footer.svelte';
</script>

<NavBar />
<main>
  <Hero />
  <h2 class="cdp-h2" style="color:brown; text-align: center; margin: 8rem 2rem;">
    Note: Below are some experiments of what the new website could look like with different Mozilla
    Protocol components.
  </h2>
  <SplitContainer />
  <SplitContainerDark />
  <CallOut />
  <EmphasisBox />
  <h2 class="cdp-h2" style="color:brown; text-align: center;">
    Note: Below is a Svelte implementation of the old website.
  </h2>
  <About />
  <Instances />
  <Contributing />
</main>
<Footer />

<style>
  .cdp-h2 {
    font-family: 'Urbanist', Arial, Helvetica, sans-serif;
    font-weight: 700;
  }
</style>
