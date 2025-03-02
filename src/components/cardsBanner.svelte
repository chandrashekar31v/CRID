<script lang="ts">
  // get props 1.title 2.cards and loop
  export let title;
  export let cards;
</script>

<div class="w-screen h-[700px] md:h-fit bg-gray-100 md:py-10 py-2 md:pl-14">
  <h1 class="text-blue-600 text-xl md:text-4xl font-semibold">{title}</h1>

  <!-- loop cards -->
  <div class="flex justify-between md:mt-16">
    {#each cards as card}
      <div class="md:w-1/5 w-1/4 md:min-h-[400px] md:h-fit h-[600px] md:mr-6 md:px-8 pt-2 bg-white rounded-md">
        <h1 class="text-2xl font-semibold md:mt-4">{card?.title}</h1>
        <p class="md:text-lg text-base font-normal">{card?.description}</p>
      </div>
    {/each}
  </div>
</div>
