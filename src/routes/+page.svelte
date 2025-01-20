<!-- Home page -->

<script>
  import SliderFloor from "../components/SliderFloor.svelte";
  import AboutUs from "../components/AboutUs.svelte";
  import CardsBanner from "../components/cardsBanner.svelte";
  import {
    WorkForceManagement,
    ITManagedServices,
  } from "../resources/data/cardsData";
  import ImageTextBanner from "../components/imageTextBanner.svelte";
  import { data } from "../resources/data/imageTextData";
  import aboutUs1 from "../resources/images/about-us-1.png"
  import aboutUs2 from "../resources/images/about-us-2.jpg"
  import aboutUs3 from "../resources/images/about-us-3.webp"
  import aboutUs4 from "../resources/images/about-us-4.jfif"

  const list = [aboutUs1,aboutUs2,aboutUs3,aboutUs4];

</script>

<div class="w-screen p-0 m-0">
  <!-- Top Slider -->
  <SliderFloor />

  <!-- About Us -->
  <AboutUs />

  <!-- cards banner -->
  <div class="hidden md:block">
    <CardsBanner cards={WorkForceManagement} title="Work For Management" />
  <CardsBanner cards={ITManagedServices} title="IT Managed Services" />
  </div>

  <!-- Image Text Banner -->
  {#each data as item, index}
    <ImageTextBanner
      image={list[index]}
      imagePosition={index % 2 === 0 ? "left" : "right"}
      data={item}
    />
  {/each}
</div>
