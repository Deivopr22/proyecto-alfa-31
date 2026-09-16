<script>
    import Icon from '@iconify/svelte';
    import summarycontent from '$lib/components/summarycontent.svelte';
</script>


<section class="py-54 flex-col gap-12 justify-start items-stretch grid grid-cols-1 px-4 md:px-12 lg:px-24">
    <div class="items-start gap-4 flex flex-col">
        <h1 class="font-montserrat text-7xl font-bold">Summary</h1>
        <p class="font-montserrat text-gray-600">A meticulous record of professional engagements, academic pursuits, and acquired competencies, emphasizing structural clarity and editorial precision</p>
        <a href="/cv.pdf" class="bg-black text-white px-4 py-2 flex font-montserrat items-center gap-2"> <Icon icon ="akar-icons:download" class="text-base"/> Download PDF</a>
    </div>

    <hr class="border-gray-300 border-t-2 w-full"/>

   
    <div class="flex gap-8">
        <p class="font-montserrat text-2xl">Experience</p>
        <p class="font-montserrat text-md">2021 - Present</p>
        <h2 class="font-montserrat text-2xl font-bold">Lead Architect</h2>
        <p class="font-montserrat text-lg">Directed comprehensive spatial design projects focusing on reductive geometry and material purity.</p>
    
    </div>
</section>