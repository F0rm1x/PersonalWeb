<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
<script>
  import "../app.css";
</script>
<nav class="bg-black pl-9 pr-9">
  <div class="space-x-4 md:flex">
    <a href="/" class="hover:bg-gray-500 space-x-4 p-4 text-xl text-white hover:text-gray-900">Home</a>
    <a href="/test" class="hover:bg-gray-500 space-x-4 p-4 text-xl text-white hover:text-gray-900">Test</a>
  </div>
</nav>
<main>
<slot />
</main>
<style lang="postcss">
  :global(html) {
    background-color: theme(colors.black);
    color: theme('colors.gray.800')
  }
</style>