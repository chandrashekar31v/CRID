<script lang="ts">
  // get props 1.title 2.cards and loop
  export let title;
  export let cards;
</script>

<div class="w-screen h-[600px] bg-gray-100 py-10 pl-14">
  <h1 class="text-blue-600 text-4xl font-semibold">{title}</h1>

  <!-- loop cards -->
  <div class="flex justify-between mt-16">
    {#each cards as card}
      <div class="w-1/6 h-[400px] mr-6 px-8 pt-2 bg-white rounded-md">
        <h1 class="text-2xl font-semibold mt-4">{card?.title}</h1>
        <p class="text-lg font-normal">{card?.description}</p>
      </div>
    {/each}
  </div>
</div>
