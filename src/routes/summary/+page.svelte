<script lang="ts">
  import Icon from '@iconify/svelte';
  import SummarySection from '$lib/components/summarycontent.svelte';
  import { summaryinfo } from '$lib/data/summaryinfo.js';
</script>

<section class="max-w-7xl mx-auto px-6 md:px-12 lg:px-24 py-16">
  
  <div class="max-w-xl space-y-6 mb-16">
    <h1 class="font-montserrat text-6xl md:text-7xl font-bold text-black">
      Summary
    </h1>
    <p class="text-gray-600 text-sm md:text-base font-light leading-relaxed">
      A meticulous record of professional engagements, academic pursuits, and acquired competencies, emphasizing structural clarity and editorial precision.
    </p>
    <a 
      href="/cv.pdf" 
      download
      class="inline-flex items-center gap-3 bg-black text-white text-xs font-semibold uppercase tracking-widest px-6 py-3.5 hover:bg-gray-800 transition-colors"
    >
      DOWNLOAD PDF
      <Icon icon="akar-icons:download" class="text-sm" />
    </a>
  </div>

  <hr class="border-gray-200 border-t w-full" />

  <SummarySection title="Experience" items={summaryinfo.experience} />

  <SummarySection title="Education" items={summaryinfo.education} />

  <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 py-16 border-b border-gray-200">
    <div class="lg:col-span-3">
      <h2 class="font-serif text-2xl md:text-3xl font-normal text-gray-900">
        Skills
      </h2>
    </div>
    
    <div class="lg:col-span-9 flex flex-wrap gap-3">
      {#each summaryinfo.skills as skill}
        <span class="border border-gray-300 px-3 py-2 text-[10px] font-semibold uppercase tracking-widest text-gray-800 bg-gray-50/50">
          {skill}
        </span>
      {/each}
    </div>
  </div>

</section>