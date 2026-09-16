<script>
    import Icon from '@iconify/svelte';
</script>

<section class="max-w-7xl mx-auto px-4 md:px-12 lg:px-24 py-16 flex flex-col gap-12">
    <!-- Encabezado -->
    <div class="items-start gap-4 flex flex-col max-w-2xl">
        <h1 class="font-serif font-bold text-5xl md:text-7xl">
            Let's work together.
        </h1>

        <p class="font-serif text-gray-600 text-base md:text-xl tracking-wide">
            We are always looking for new opportunities to collaborate and create meaningful experiences. If you have a project in mind, feel free to reach out to us.
        </p>
    </div>

    <!-- Grilla principal de 2 columnas (Info a la izquierda, Formulario a la derecha) -->
    <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 pt-6">
        
        <!-- COLUMNA IZQUIERDA (Ocupa 4 columnas de 12) -->
        <div class="lg:col-span-4 flex flex-col gap-8">
            <div class="flex flex-col gap-2">
                <h3 class="font-sans text-gray-500 text-xs font-bold uppercase tracking-widest">contact details</h3>
                <p class="font-sans text-xs font-bold text-gray-800">deivisp563@gmail.com</p>
                <p class="font-sans text-xs font-bold text-gray-800">+58 (412)-7467276</p>
            </div>

            <div class="flex flex-col gap-2">
                <h3 class="font-sans text-gray-500 text-xs font-bold uppercase tracking-widest">location</h3>
                <p class="font-sans text-xs font-bold text-gray-800">1234 Main Street</p>
                <p class="font-sans text-xs font-bold text-gray-800">City, State 12345</p>
                <p class="font-sans text-xs font-bold text-gray-800">New York, NY 10001</p>
            </div>

            <div class="flex flex-col gap-2 items-start">
                <h3 class="font-sans text-gray-500 text-xs font-bold uppercase tracking-widest">social</h3>
                <a href="https://www.linkedin.com/in/deivis-p%C3%A9rez-444045342/" target="_blank" class="underline underline-offset-4 hover:text-gray-500 text-xs font-bold">LinkedIn</a>
                <a href="https://github.com/Deivopr22" target="_blank" class="underline underline-offset-4 hover:text-gray-500 text-xs font-bold">GitHub</a>
                <a href="https://www.instagram.com/deivopr22/" target="_blank" class="underline underline-offset-4 hover:text-gray-500 text-xs font-bold">Instagram</a>
            </div>
        </div>

        <!-- COLUMNA DERECHA: FORMULARIO (Ocupa 8 columnas de 12) -->
        <div class="lg:col-span-8">
            <form onsubmit={(e) => e.preventDefault()} class="flex flex-col gap-6">
                <div class="flex flex-col gap-2">
                    <label for="fname" class="font-sans text-gray-500 text-xs font-bold uppercase tracking-widest">NAME</label>
                    <input 
                        type="text" 
                        id="fname" 
                        name="fname" 
                        placeholder="Your full name"
                        class="border-b border-gray-300 py-2 text-sm bg-transparent focus:outline-none focus:border-black"
                    >
                </div>

                <div class="flex flex-col gap-2">
                    <label for="email" class="font-sans text-gray-500 text-xs font-bold uppercase tracking-widest">EMAIL</label>
                    <input 
                        type="email" 
                        id="email" 
                        name="email" 
                        placeholder="hello@example.com"
                        class="border-b border-gray-300 py-2 text-sm bg-transparent focus:outline-none focus:border-black"
                    >
                </div>

                <div class="flex flex-col gap-2">
                    <label for="message" class="font-sans text-gray-500 text-xs font-bold uppercase tracking-widest">MESSAGE</label>
                    <textarea 
                        id="message" 
                        name="message" 
                        rows="4" 
                        placeholder="Tell us about your project..."
                        class="border-b border-gray-300 py-2 text-sm bg-transparent focus:outline-none focus:border-black resize-none"
                    ></textarea>
                </div>

                <div class="pt-4">
                    <button 
                        type="submit" 
                        class="bg-black text-white text-xs font-bold uppercase tracking-widest px-8 py-4 hover:bg-gray-800 transition-colors"
                    >
                        Send Message
                    </button>
                </div>
            </form>
        </div>

    </div>
</section>