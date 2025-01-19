<script lang="ts">
  export let image;
  export let imagePosition;
  export let data;
  export let className="";
</script>

<div class={`flex w-screen mt-14 h-[450px] mb-2 px-40 ${className}`}>
  {#if imagePosition === "left"}
    <div
      class="w-2/5 h-[350px] bg-no-repeat bg-cover"
      style="background-image: url({image})"
    ></div>
  {/if}
  <div class="w-3/5 p-3">
    <h1 class="text-blue-600 font-bold text-3xl pb-4">{@html data?.title}</h1>
    <p class="text-lg leading-8">{@html data?.description}</p>
  </div>
  {#if imagePosition === "right"}
    <div
      class="w-2/5 h-[350px] bg-no-repeat bg-right-top bg-cover"
      style="background-image: url({image})"
    ></div>
  {/if}
</div>
