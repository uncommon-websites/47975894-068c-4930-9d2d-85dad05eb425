<script lang="ts">
  const cards = [
    {
      title: "We're Not Just a Vendor...",
      subtitle: "We're an Extension of Your Team.",
      image: "/generated/image-corporate-real-estate-professionals-coll-1765573359643-6.webp"
    },
    {
      title: "We Don't Fragment Services...",
      subtitle: "We Deliver End-to-End Integration.",
      image: "/generated/image-diverse-business-team-reviewing-architec-1765573362278-7.webp"
    },
    {
      title: "We Don't Just Execute...",
      subtitle: "We Transform Challenges Into Advantages.",
      image: "/generated/image-global-business-professionals-in-modern--1765573365184-8.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-2xl mb-16">
    <p class="text-xl md:text-2xl leading-relaxed text-gray-800">
      Corporate real estate directors face a common challenge: fragmented vendor relationships that drain resources. We consolidate everything under one roof, becoming your trusted partner from strategy through execution.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each cards as card}
      <div class="group">
        <div class="aspect-[4/3] overflow-hidden rounded-lg mb-4 bg-gray-100">
          <img src={card.image} alt={card.title} class="w-full h-full object-cover grayscale group-hover:grayscale-0 transition-all duration-500" />
        </div>
        <h3 class="text-sm text-gray-500 mb-1">{card.title}</h3>
        <p class="text-sm font-bold">{card.subtitle}</p>
        
        <div class="flex justify-between mt-4 text-xs text-gray-400">
           <span>01</span>
           <span>-></span>
        </div>
      </div>
    {/each}
  </div>
</section>
