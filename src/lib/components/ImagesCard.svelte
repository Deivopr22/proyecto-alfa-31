<script>
    let {name, category, image, id, slug} = $props()
</script>


<a href={"/projects/" + slug} class="group block cursor-pointer">
    <article class="flex flex-col h-full">
        <div class="w-full aspect-square bg-gray-100 overflow-hidden mb-6">
            <img 
                src={image} 
                alt={name} 
                class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-700 ease-out"
            />
        </div>

        <div class="flex flex-col items-start gap-3">
            <span class="border border-gray-300 px-2.5 py-1 text-[10px] font-semibold uppercase tracking-widest text-gray-500 bg-transparent">
                {category}
            </span>
            <h3 class="font-montserrat text-lg text-gray-900">
                {name}
            </h3>
        </div>
    </article>
</a>