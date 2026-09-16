<script>
    import ImagesCard from '$lib/components/ImagesCard.svelte';

    const projects = [
    {
      name: 'The Void Residence',
      category: 'ARCHITECTURE',
      image: '/images/project1.jpg'
    },
    {
      name: 'Monochrome Magazine Vol. II',
      category: 'PRINT / EDITORIAL',
      image: '/images/project2.jpg'
    },
    {
      name: 'Object 04',
      category: 'INDUSTRIAL DESIGN',
      image: '/images/project3.jpg'
    },
    {
      name: 'Form Studies',
      category: 'DIGITAL ART',
      image: '/images/project4.jpg'
    },
    {
      name: 'Gallery Space Layout',
      category: 'INTERIOR',
      image: '/images/project5.jpg'
    },
    {
      name: 'FW24 Campaign',
      category: 'ART DIRECTION',
      image: '/images/project6.jpg'
    }
  ];
</script>

<div class="w-full max-w-7xl mx-auto px-6 md:px-12 py-12">
    <section class="mb-16 max-w-xl space-y-4">
        <h1 class="font-serif text-5xl md:text-6xl font-bold">Selected Works</h1>
        <p class="text-gray-600 text-base md:text-lg font-light leading-relaxed">A curated collection of recent projects exploring minimalism, editorial layout, and spatial design.</p>
    </section>
</div>

<section class="grid grid-cols-1 md:grid-cols-3 gap-x-8 gap-y-12">
    {#each projects as project}
      <ImagesCard
        name={project.name}
        category={project.category}
        image={project.image}
      />
    {/each}
  </section>