<script lang="ts">
  const stats = [
    {
      label: "18,000+ Employees Globally",
      desc: "With 500+ dedicated corporate real estate professionals and 18,000 total employees worldwide, we combine global scale with local expertise. Our team spans 30 offices across North America, Europe, Middle East, Africa, and Asia-Pacific, delivering integrated solutions wherever your business operates.",
      img: "/generated/image-corporate-office-team-working-together-i-1765573371023-10.webp"
    },
    {
      label: "Award-Winning Excellence",
      desc: "Recognized on Inc. 5000's Fastest-Growing Private Companies (2024), India's Top 50 Best Workplaces for Women, and multiple MUSE Design Awards. Our Frost & Sullivan Customer Value Leadership Award reflects our commitment to client success and innovation in corporate real estate.",
      img: "/generated/image-professional-business-meeting-in-modern--1765573373836-11.webp"
    },
    {
      label: "30 Global Offices",
      desc: "Headquartered in Chicago, with major hubs in Bangalore, Shanghai, London, New York, Los Angeles, Dallas, Detroit, and Charlotte. Our strategic global presence ensures we understand local markets while delivering consistent, world-class service across every region.",
      img: "/generated/image-global-business-professionals-in-modern--1765573365184-8.webp"
    },
    {
      label: "Fortune 500 Trust",
      desc: "From emerging startups to Fortune 500 companies, we serve corporate clients exclusively across Industrial, Healthcare, Financial Services, Retail, and Office sectors. Our people-first approach and transparency-driven culture have made us the trusted partner for companies transforming their real estate portfolios.",
      img: "/generated/image-diverse-corporate-team-celebrating-succe-1765573376590-12.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white border-t border-gray-100">
  <div class="mb-16">
    <p class="text-gray-500 max-w-xl">
      Discover the scale, expertise, and recognition that makes Vestian the trusted partner for corporate real estate transformation.
    </p>
  </div>

  <div class="space-y-16">
    {#each stats as stat}
      <div class="flex flex-col md:flex-row md:items-start justify-between gap-8 border-b border-gray-100 pb-16 last:border-0">
        <h3 class="text-2xl md:text-4xl font-medium w-full md:w-1/3">{stat.label}</h3>
        <div class="w-full md:w-1/3">
           <p class="text-xs leading-relaxed text-gray-500">{stat.desc}</p>
        </div>
        <div class="w-full md:w-1/6 flex justify-end">
           <img src={stat.img} alt={stat.label} class="w-20 h-20 object-cover rounded bg-gray-100" />
        </div>
      </div>
    {/each}
  </div>
</section>
