<script lang="ts">
  type Item = {
    timeline: string;
    role: string;
    company: string;
    description: string;
  };

  let { title, items }: { title: string; items: Item[] } = $props();
</script>

<div class="grid grid-cols-1 lg:grid-cols-12 gap-8 py-16 border-b border-gray-200">
  <div class="lg:col-span-3">
    <h2 class="font-serif text-2xl md:text-3xl font-normal text-gray-900">
      {title}
    </h2>
  </div>

  <div class="lg:col-span-9 flex flex-col divide-y divide-gray-200">
    {#each items as item, index}
      <div class="grid grid-cols-1 md:grid-cols-12 gap-6 {index !== 0 ? 'pt-10 mt-10' : ''}">
        
        <div class="md:col-span-4">
          <span class="text-xs uppercase tracking-widest text-gray-500 font-sans">
            {item.timeline}
          </span>
        </div>
        
        <div class="md:col-span-8 space-y-2 pb-8">
          <h3 class="font-serif text-2xl text-gray-900 font-normal">
            {item.role}
          </h3>
          <p class="text-xs text-gray-500 font-sans">
            {item.company}
          </p>
          <p class="text-sm text-gray-600 font-light leading-relaxed pt-2">
            {item.description}
          </p>
        </div>

      </div>
    {/each}
  </div>
</div>