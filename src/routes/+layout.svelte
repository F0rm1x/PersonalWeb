<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
<script>
  import "../app.css";
</script>
<nav class="bg-gray-800 pl-9 pr-9">
  <div class="block md:flex md:space-x-6">
    <a href="/" class="hover:bg-gray-500 p-2 text-xl text-white hover:text-gray-900">Home</a>
    <a href="/test" class="hover:bg-gray-500  p-2 text-xl text-white hover:text-gray-900">Test</a>
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