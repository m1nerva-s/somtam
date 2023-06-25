<svelte:head>
    <title>เว็บส้มตำ</title> 
</svelte:head>

<script>
  import { somtamList } from "../somtamList";
  // import { Card } from "../components/Card.svelte";
</script>

<div class="w-screen min-h-screen bg-black align-middle">
  <div class="w-screen bg-black p-6 pl-8 md:pl-16 border-b-4 border-primary mb-16">
    <img src="icon_somtam.png" class="w-32" alt="logo" />
  </div>
  <div class="container mx-auto">
    <div class="flex flex-wrap justify-center">
      {#each somtamList as somtam}
        <div class="px-4 mb-8">
          <div class=" px-4 mb-8">
            <div class="relative w-full h-fit">
              <img style="max-width:300px;" class="aspect-video object-fill" src={somtam.img} alt={somtam.somtamName}>
            </div>
            <div class="mt-2">
              <h2 class="text-xl font-semibold text-white">{somtam.somtamName}</h2>
            </div>
          </div>
          </div>
      {/each}
    </div>
  </div>
</div>
