<script>
  import NavBar from '$lib/NavBar.svelte';
  import Footer from '$lib/Footer.svelte';
  import ContactSection from '$lib/ContactSection.svelte';
  import AboutSection from '$lib/AboutSection.svelte';
  import ProjectsSection from '$lib/ProjectsSection.svelte';
</script>

<NavBar />

<section id="home" class="container mx-auto mt-10">
  <h2 class="text-4xl font-bold mb-4">Welcome to My Portfolio</h2>
</section>


<div class="p-4">
  <div class="border-4 border-red-500 p-4">
    <img src="https://media.tenor.com/9n1CXysOWEAAAAAj/ethosaur-nonagon.gif" alt="Website under construction" class="mx-auto" />
    <h1 class="text-center text-4xl font-bold mt-10">This website is under construction!</h1>
  </div>
</div>


<AboutSection />

<ProjectsSection />

<ContactSection />

<Footer />
