<script>
    import ImagesCard from '$lib/components/ImagesCard.svelte';
    import { projects } from '$lib/data/projects';
    
</script>

<div class="w-full max-w-7xl mx-auto px-6 md:px-12 py-12">
    <section class="mb-16 max-w-xl space-y-4">
        <h1 class="font-montserrat text-5xl md:text-6xl font-bold">Selected Works</h1>
        <p class="text-gray-600 text-base md:text-lg font-light leading-relaxed">A curated collection of recent projects exploring minimalism, editorial layout, and spatial design.</p>
    </section>
</div>

<section class="grid grid-cols-1 md:grid-cols-3 gap-x-8 gap-y-12">
    {#each projects as project}
      <ImagesCard
        name={project.name}
        category={project.category}
        image={project.image}
        id={project.id}
        slug={project.slug}
      />
    {/each}
  </section>