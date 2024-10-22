<script>
  import ProjectCard from '$lib/ProjectCard.svelte';

  let projects = [
    { title: "Project 1", description: "This is project 1", link: "#" },
    { title: "Project 2", description: "This is project 2", link: "#" },
    { title: "Project 3", description: "This is project 3", link: "#" },
    { title: "Project 1", description: "This is project 1", link: "#" },
    { title: "Project 2", description: "This is project 2", link: "#" },
    { title: "Project 3", description: "This is project 3", link: "#" }
  ];
</script>

<section id="projects" class="container mx-auto mt-10">
  <h2 class="text-4xl font-bold mb-4">Projects</h2>
  <div class="flex flex-wrap">
    {#each projects as project}
      <ProjectCard title={project.title} description={project.description} link={project.link} />
    {/each}
  </div>
</section>