<script>
    import Icon from '@iconify/svelte';
</script>

<section class="w-full max-w-7xl mx-auto px-6 md:px-12 py-16 lg:py-24">
    <div class="flex lg:grid grid-cols-1 lg:grid-cols-12 gap-12 lg:gap-16 items-start-span-5 gap-5">
       <div class="lg:col-span-5">
            <div class="w-full aspect-[4/5] bg-gray-100 overflow-hidden">
                <img 
                src="/profile.jpg" 
                alt="Retrato" 
                class="w-full h-full object-cover grayscale"
                />
            </div>
       </div>

       <div class="lg:col-span-6 lg:col-start-7 flex flex-col">
            <div class="mb-8 space-y-4">
                <h1 class="font-montserrat text-5xl md:text-6xl text-black font-bold ">
                    About me.
                </h1>
            </div>

            <div class="space-y-6 text-gray-600 text-sm md:text-base font-light leading-relaxed">
                <p>
                    I am a multidisciplinary designer focused on creating digital experiences that strip away the unnecessary. My work is rooted in the belief that true luxury lies in clarity, precision, and the masterful use of negative space.
                </p>
                <p>
                    With a background spanning editorial design, architecture, and digital interfaces, I approach every project as a structural puzzle. The goal is never to decorate, but to reveal the core essence of the brand or product through rigorous typography and intentional grid systems.
                </p>
            </div>

            <hr class="border-gray-200 my-10 w-full" />

            <div class="space-y-4 mb-12">
                <h2 class="text-xs font-semibold uppercase tracking-[0.2em] text-gray-900 font-sans">
                    Design Philosophy
                </h2>
                <p class="text-gray-600 text-sm font-light leading-relaxed">
                    Minimalism is not an aesthetic choice; it is a functional requirement. By removing noise, we amplify the signal. Every line, every pixel, and every margin must serve a distinct purpose or be ruthlessly eliminated.
                </p>
            </div>

            <div class="flex gap-8">
                <a href="https://www.instagram.com/deivopr22" target="_blank" class="group flex items-center gap-2 text-[10px] uppercase tracking-widest font-semibold text-gray-500 hover:text-black transition-colors">
                    <Icon icon="lucide:arrow-up-right" class="text-sm group-hover:-translate-y-0.5 group-hover:translate-x-0.5 transition-transform" />
                    Instagram
                </a>
                <a href="https://github.com/Deivopr22" target="_blank" class="group flex items-center gap-2 text-[10px] uppercase tracking-widest font-semibold text-gray-500 hover:text-black transition-colors">
                    <Icon icon="lucide:arrow-up-right" class="text-sm group-hover:-translate-y-0.5 group-hover:translate-x-0.5 transition-transform" />
                    GitHub
                </a>
            </div>
       </div>
    </div>
   

   
</section>