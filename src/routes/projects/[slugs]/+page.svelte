<script>
    import { projects } from '$lib/data/projects';

    const { params } = $props()

    const ProjectData = projects.find(
        project => project.slug == params.slugs
    )

</script>

{#if ProjectData}
    <section class="w-full max-w-7xl mx-auto px-6 md:px-12 py-12">
        <h1 class="font-montserrat text-5xl md:text-6xl font-bold">{ProjectData.name}</h1>
        <p class="text-gray-600 text-base md:text-lg font-light leading-relaxed">{ProjectData.category}</p>
    </section>

    <section class="w-full max-w-7xl mx-auto px-6 md:px-12 py-12">
        <img src={ProjectData.image} alt={ProjectData.name} class="w-full h-auto object-cover" />
    </section>
{/if}