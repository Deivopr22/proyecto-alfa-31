<script>

    const {name, category, image} = $props()

</script>

<section>

    <article class="group flex flex-col space-y-4 cursor-pointer">
        <div class="w-full aspect-square bg-gray-100 overflow-hidden">
            <img src={image} alt={name} class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500 ease-out" />
        </div>
    </article>

    <div class="space-y-2 text-left">
        <h3 class="font-bold text-lg">{name}</h3>
        <p class="text-gray-600">{category}</p>
    </div>
</section>