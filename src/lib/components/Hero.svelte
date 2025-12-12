<script lang="ts">
  // Client logos - Fortune 500 companies and major brands
  const logos = [
    "JPMC",
    "Credit Suisse",
    "DBS",
    "Cetera",
    "Fannie May"
  ];
</script>

<section class="relative min-h-screen flex flex-col justify-end pb-20 px-6 md:px-12 bg-gradient-to-b from-[#1a1a1a] via-[#2a2a2a] to-[#fdfbf7] text-[#1a1a1a]">
  <!-- Gradient overlay/background handling -->
  <div class="absolute inset-0 z-[-1] bg-[linear-gradient(180deg,#0a0a0a_0%,#1a1a1a_30%,#3a3a3a_60%,#fff_100%)]"></div>

  <div class="max-w-4xl mb-32 pt-40">
    <h1 class="text-3xl md:text-5xl font-medium leading-[1.15] tracking-tight text-white">
      Transforming corporate real estate portfolios through integrated global advisory and execution services. <span class="text-gray-400">We serve Fortune 500 companies and growing enterprises, delivering end-to-end solutions that turn real estate challenges into business advantages.</span>
    </h1>
  </div>

  <div class="border-t border-gray-300 pt-8 flex flex-wrap gap-8 md:gap-16 items-center opacity-60 grayscale">
    {#each logos as logo}
      <div class="h-8 flex items-center justify-center font-bold text-xl text-white">{logo}</div>
    {/each}
    <!-- Add more specific logo placeholders if needed -->
    <div class="h-8 w-20 bg-gray-400/20 rounded"></div>
    <div class="h-8 w-20 bg-gray-400/20 rounded"></div>
    <div class="h-8 w-20 bg-gray-400/20 rounded"></div>
  </div>
</section>
