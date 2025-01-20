<script lang="ts">
  export let image;
  export let imagePosition;
  export let data;
  export let className="";
</script>

<div class={`md:flex w-screen md:mt-14 md:h-[450px] h-fit mb-2 md:px-40 px-10 ${className}`}>
  {#if imagePosition === "left"}
    <div
      class="md:w-2/5 md:h-[350px] h-[200px] bg-no-repeat bg-cover"
      style="background-image: url({image})"
    ></div>
  {/if}
  <div class="md:w-3/5 p-3">
    <h1 class="text-blue-600 font-bold text-3xl pb-4">{@html data?.title}</h1>
    <p class="text-lg leading-8">{@html data?.description}</p>
  </div>
  {#if imagePosition === "right"}
    <div
      class="md:w-2/5 md:h-[350px] h-[200px] bg-no-repeat bg-right-top bg-cover"
      style="background-image: url({image})"
    ></div>
  {/if}
</div>
