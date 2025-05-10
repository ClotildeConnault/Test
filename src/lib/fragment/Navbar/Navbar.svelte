<script lang="ts">
  export let scrolled = false;
</script>

<nav
  class="{scrolled
    ? 'bg-black/40'
    : 'bg-transparent'} fixed top-0 z-50 h-16 w-full flex text-white text-xl
  justify-end items-center px-4 transition-colors duration-300 select-none"
>
  <!-- <img class="h-20 pt-5" src="/logo-blanc.png" alt="logo"> -->
  <ul class="flex justify-between gap-4">
    <li><a class=" hover:text-blue-950" href="/">Accueil</a></li>
    <li>
      <a class=" hover:text-blue-950" href="/presentation">Qui sommes-nous ?</a>
    </li>
    <li><a class=" hover:text-blue-950" href="/contact">Contact</a></li>
  </ul>
</nav>
