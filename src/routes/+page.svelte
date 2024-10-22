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

<AboutSection />

<ProjectsSection />

<ContactSection />

<Footer />
