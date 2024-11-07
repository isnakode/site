<script>
  import { apps, fws, langs, sosmed, tools } from "$lib/skills";
</script>

<main class="p-8 flex flex-col items-center text-center">
  <h1 class="text-3xl font-semibold mb-8">IsnaKode</h1>
  <p>
    Kumpulan
    <span class="bg-red-400 text-white p-1.5 pt-0.5 rounded-md">
      Portfolio
    </span>
    oleh
    <span class="bg-blue-500 text-white p-1.5 pt-0.5 rounded-md">
      Muhammad isnaini
    </span>
  </p>
  <h2 class="text-2xl font-medium my-8">Sosial media</h2>
  <div class="flex flex-wrap justify-center gap-8">
    {#each sosmed as { link, icon }}
      <div class="size-8 hover:scale-125 transition-all">
        <a href={link} target="_blank">
          <img src={icon} class="size-full" alt="sosial media" /></a
        >
      </div>
    {/each}
  </div>
  <h2 class="text-2xl font-medium my-8">Aplikasi dan tool yang dibuat</h2>
  <div class="flex flex-wrap justify-center gap-8">
    {#each apps as { title, icon }}
      <div
        class="size-16 md:size-24 rounded-xl overflow-hidden hover:scale-125 transition-all"
      >
        <img src={icon} alt={title} />
      </div>
    {/each}
  </div>
  <h2 class="text-2xl font-medium my-8">Bahasa pemrograman</h2>
  <div class="flex flex-wrap justify-center gap-8">
    {#each langs as { title, icon }}
      <div
        class="size-16 md:size-24 rounded-xl overflow-hidden hover:scale-125 transition-all"
      >
        <img src={icon} alt={title} />
      </div>
    {/each}
  </div>
  <h2 class="text-2xl font-medium my-8">Framework</h2>
  <div class="flex flex-wrap justify-center gap-8">
    {#each fws as { title, icon }}
      <div
        class="size-16 md:size-24 rounded-xl overflow-hidden hover:scale-125 transition-all"
      >
        <img src={icon} alt={title} class="size-full" />
      </div>
    {/each}
  </div>
  <h2 class="text-2xl font-medium my-8">Tools</h2>
  <div class="flex flex-wrap justify-center gap-8">
    {#each tools as { title, icon }}
      <div
        class="size-16 md:size-24 rounded-xl overflow-hidden hover:scale-125 transition-all"
      >
        <img src={icon} alt={title} class="size-full" />
      </div>
    {/each}
  </div>
</main>
