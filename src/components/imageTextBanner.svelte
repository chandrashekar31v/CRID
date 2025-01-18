<script lang="ts">
  export let image;
  export let imagePosition;
  export let data;
</script>

<div class="flex w-screen mt-14 h-[450px] mb-2 px-40">
  {#if imagePosition === "left"}
    <div
      class="w-2/5 h-[350px] bg-no-repeat"
      style="background-image: url({image})"
    ></div>
  {/if}
  <div class="w-3/5 p-3">
    <h1 class="text-blue-600 font-bold text-3xl pb-4">{data?.title}</h1>
    <p class="text-lg leading-8">{data?.description}</p>
  </div>
  {#if imagePosition === "right"}
    <div
      class="w-2/5 h-[350px] bg-no-repeat bg-right-top"
      style="background-image: url({image})"
    ></div>
  {/if}
</div>
