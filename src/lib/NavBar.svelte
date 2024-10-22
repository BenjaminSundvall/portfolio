<script>
  let links = [
    { name: "Home", path: "#home" },
    { name: "About", path: "#about" },
    { name: "Projects", path: "#projects" },
    { name: "Contact", path: "#contact" }
  ];
</script>

<!-- Add fixed, w-full, and top-0 to keep it at the top -->
<nav class="fixed top-0 left-0 w-full bg-gray-800 text-white p-4 z-50 shadow-lg">
  <div class="container mx-auto flex justify-between items-center">
    <a href=/ class="text-xl font-bold">Benjamin Sundvall</a>
    <ul class="flex space-x-4">
      {#each links as link}
        <li>
          <a href={link.path} class="hover:text-gray-400 transition">{link.name}</a>
        </li>
      {/each}
    </ul>
  </div>
</nav>

<!-- Add padding to the top of the body to prevent content overlap with the fixed navbar -->
<div class="pt-16"></div>