<script>
  import { fly, fade } from 'svelte/transition';

  export let title;
  export let description;
  export let link;
</script>

<div
  class="max-w-sm rounded overflow-hidden shadow-lg bg-white m-4"
  in:fly={{ x: 200, duration: 500 }}
  out:fade={{ duration: 300 }}
>
  <div class="px-6 py-4">
    <div class="font-bold text-xl mb-2">{title}</div>
    <p class="text-gray-700 text-base">{description}</p>
  </div>
  <div class="px-6 pt-4 pb-2">
    <a href={link} target="_blank" class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
      View Project
    </a>
  </div>
</div>
