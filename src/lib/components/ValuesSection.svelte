<script lang="ts">
  const photos = [
    {
      title: "Collaborative Excellence",
      desc: "Our people-first approach creates an environment where ideas shape the future of corporate real estate.",
      img: "/generated/image-corporate-office-team-working-together-i-1765573371023-10.webp"
    },
    {
      title: "Transparency & Trust",
      desc: "Commitment to transparency and client success drives all our operations, building lasting partnerships.",
      img: "/generated/image-professional-business-meeting-in-modern--1765573373836-11.webp"
    },
    {
      title: "Inclusive Culture",
      desc: "Recognized as one of India's Top 50 Best Workplaces for Women, we foster trust-based, inclusive teams.",
      img: "/generated/image-diverse-corporate-team-celebrating-succe-1765573376590-12.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-xl mb-16">
    <h3 class="text-lg font-bold mb-2">We focus on people, not just portfolios.</h3>
    <p class="text-gray-500 text-sm leading-relaxed">
      Our culture is built on transparency, collaboration, and a people-first philosophy. Led by CEO Shrinivas Rao—recognized as one of India's Top 50 Great People Managers—we create inclusive, trust-based workplaces where every team member contributes to transforming corporate real estate challenges into business advantages.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each photos as photo}
      <div>
        <div class="aspect-[3/4] rounded-lg overflow-hidden mb-4 bg-gray-100">
          <img src={photo.img} alt={photo.title} class="w-full h-full object-cover" />
        </div>
        <h4 class="text-xs font-bold mb-1">{photo.title}</h4>
        <p class="text-[10px] text-gray-500 leading-relaxed">{photo.desc}</p>
      </div>
    {/each}
  </div>
</section>
