<!-- Home page -->

<script>
  import Header from "../components/Header.svelte";
  import SliderFloor from "../components/SliderFloor.svelte";
  import AboutUs from "../components/AboutUs.svelte";
  import CardsBanner from "../components/cardsBanner.svelte";
  import {
    WorkForceManagement,
    ITManagedServices,
  } from "../resources/data/cardsData";
  import ImageTextBanner from "../components/imageTextBanner.svelte";
  import { data } from "../resources/data/imageTextData";
  import aboutUs from "../resources/images/aboutUs.png"
</script>

<div>
  <!-- header -->
  <Header />

  <!-- Top Slider -->
  <SliderFloor />

  <!-- About Us -->
  <AboutUs />

  <!-- cards banner -->
  <CardsBanner cards={WorkForceManagement} title="Work For Management" />
  <CardsBanner cards={ITManagedServices} title="IT Managed Services" />

  <!-- Image Text Banner -->
  {#each data as item, index}
    <ImageTextBanner
      image={aboutUs}
      imagePosition={index % 2 === 0 ? "left" : "right"}
      data={item}
    />
  {/each}
</div>
