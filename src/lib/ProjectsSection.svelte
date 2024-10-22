<script>
  import ProjectCard from '$lib/ProjectCard.svelte';

  let projects = [
    { title: "Project 1",
      description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
      link: "#",
      image:  "https://1.bp.blogspot.com/-5hXynezmCxk/YQrXexMlkwI/AAAAAAAAQxk/NHTz5XwLCR4xPyDHEwUiMgPk1sFRANrlQCLcBGAsYHQ/s0/Clipart%2BRender%2BWall%2BE%2By%2BEva%2BPNG%2BDescarga%2Bgratis%2B%252817%2529.png"
    },
    { title: "Project 2",
      description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
      link: "#",
      image: "https://pngimg.com/uploads/iphone_12/iphone_12_PNG23.png"
    },
    { title: "Project 3",
      description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
      link: "#"
    },
  ];
</script>

<section id="projects" class="container mx-auto mt-10">
  <h2 class="text-4xl font-bold mb-4">Projects</h2>
  <div class="scroll-container">
    {#each projects as project}
      <ProjectCard title={project.title} description={project.description} link={project.link} image={project.image}/>
    {/each}
  </div>
</section>