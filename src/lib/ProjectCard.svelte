<script>
  export let title;
  export let description;
  export let link;
  export let image;
</script>

<a
  href={link}
  target="_blank"
  class="block w-fill h-96 rounded-xl overflow-hidden m-4 transition-transform duration-300 transform hover:scale-105"
  style="background-image: url('{image}'); background-size: contain; background-repeat: no-repeat; background-position: center; box-shadow: 0 1px 18px rgba(0, 0, 0, 0.1);"
>
  <div class="px-6 py-4 bg-white bg-opacity-75 h-full flex flex-col justify-start">
    <div class="font-bold text-xl mb-2">{title}</div>
    <p class="text-gray-700 text-base w-64">{description}</p>
  </div>
</a>
