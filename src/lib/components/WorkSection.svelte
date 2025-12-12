<script lang="ts">
  const projects = [
    {
      client: "BHS Corrugated",
      desc: "25,000 sq ft Experience Center in Charlotte's Ballantyne district delivered with precision.",
      bg: "bg-gray-100",
      img: "/generated/image-modern-corporate-office-interior-with-gl-1765573340398-0.webp",
      dark: false
    },
    {
      client: "Tint World",
      desc: "Master Services Agreement supporting automotive styling franchise expansion nationwide.",
      bg: "bg-gray-200",
      img: "/generated/image-automotive-service-center-interior-with--1765573344088-1.webp",
      dark: false
    },
    {
      client: "Soleo Health",
      desc: "Rapid expansion across 20+ US locations with strategic cost optimization.",
      bg: "bg-gray-100",
      img: "/generated/image-healthcare-office-space-with-clean-moder-1765573347229-2.webp",
      dark: false
    },
    {
      client: "Fannie May",
      desc: "Rapid retail refresh delivered in just 45 days, transforming customer experience.",
      bg: "bg-gray-200",
      img: "/generated/image-retail-storefront-with-elegant-design-an-1765573350348-3.webp",
      dark: false
    },
    {
      client: "Global Semiconductor Leader",
      desc: "State-of-the-art R&D center delivered in record time with cutting-edge infrastructure.",
      bg: "bg-[#0a0a0a]",
      img: "/generated/image-state-of-the-art-research-and-developmen-1765573353638-4.webp",
      dark: true,
      full: true
    },
    {
      client: "Financial Services",
      desc: "Workspace transformations for Cetera, Credit Suisse, JPMC, and DBS.",
      bg: "bg-gray-100",
      img: "/generated/image-luxury-financial-services-office-with-so-1765573356695-5.webp",
      dark: false
    },
    {
      client: "Swarovski Shanghai",
      desc: "Crystal elegance design bringing brand identity to life in premium office space.",
      bg: "bg-gray-200",
      img: "/generated/image-luxury-financial-services-office-with-so-1765573356695-5.webp",
      dark: false
    }
  ];
</script>

<section class="px-6 md:px-12 py-24 bg-white">
  <div class="max-w-3xl mb-16">
    <h2 class="text-2xl md:text-3xl font-medium leading-tight">
      <span class="font-bold">We integrate advisory, strategy, and execution</span> to transform corporate real estate portfolios for Fortune 500 companies and growing enterprises across every sector.
    </h2>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-2 gap-x-6 gap-y-12">
    {#each projects as project}
      <div class="group cursor-pointer {project.full ? 'md:col-span-2' : ''}">
        <div class={`aspect-[4/3] w-full rounded-lg overflow-hidden relative ${project.bg} mb-4 ${project.full ? 'md:aspect-[2.5/1]' : ''}`}>
          {#if project.img}
             <img src={project.img} alt={project.client} class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" />
          {:else}
             <!-- Placeholder for logos on solid bg -->
             <div class="w-full h-full flex items-center justify-center">
                <span class={`text-2xl font-bold ${project.dark ? 'text-white' : 'text-black'}`}>{project.client} Logo</span>
             </div>
          {/if}
        </div>
        <h3 class="text-sm font-bold mb-1">{project.client}</h3>
        <p class="text-sm text-gray-600">{project.desc}</p>
      </div>
    {/each}
  </div>
</section>
