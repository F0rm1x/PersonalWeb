<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">

<script>
  import "../app.css";
  let visible = false;
</script>



<button on:click={() => (visible = !visible)} class="fixed z-50 border-2 w-20 h-20 rounded-full border-gray-600 hover:bg-paldarkerpurple/30 hover:animate-pulse m-2"><i class="fa-solid fa-bars fa-3x"></i></button>

<div class= {`transition-all duration-500 transform ${
  visible ? 'translate-x-0 opacity-100' : '-translate-x-full opacity-0'
} bg-palpurple/80 pl-5 w-1/3 h-screen z-40 fixed top-0 left-0 sm:w-1/5`}>
  <h1 class="text-5xl text-white font-bold mb-10 text-center mt-10">Menu</h1>
    <ul>
      <li><a href="/" class="hover:bg-paldarkerpurple block w-full p-2 text-3xl text-palwhite hover:text-paldark hover:animate-pulse p-5">Home</a></li>
      <li><a href="/gallery" class="hover:bg-paldarkerpurple block  p-2 text-3xl text-palwhite hover:text-paldark hover:animate-pulse p-5">Gallery</a></li>
    </ul>
    <!-- Links div -->
    <div class="bottom-10 absolute pl-5">
    <h1 class="w-full text-xl text-palwhite font-bold">Links</h1>
    <h2 class="w-full pb-3 pt-2 text-base text-palwhite">Socials</h2>
    <a href="https://discord.com/users/948139158222831637" class="mr-10"><i class="fa-brands fa-discord text-palwhite fa-xl hover:animate-pulse"></i></a>
    <a href="https://x.com/F0rmix_df" class="mr-10"><i class="fa-brands fa-twitter text-palwhite fa-xl hover:animate-pulse"></i></a>
    <h2 class="w-full text-base text-palwhite pt-3 pb-3">Work</h2>
    <a href="https://www.deviantart.com/f0rm1x" class="mr-10"><i class="fa-brands fa-deviantart text-palwhite fa-xl hover:animate-pulse"></i></a>
    <a href="https://f0rmix.itch.io/" class="mr-10"><i class="fa-brands fa-itch-io text-palwhite fa-xl hover:animate-pulse"></i></a>
    <a href="https://github.com/F0rm1x" class="mr-10"><i class="fa-brands fa-github text-paldark fa-xl hover:animate-pulse"></i></a>

    <h2 class="w-full pt-5 text-xs text-palwhite">Email: <a href="mailto:dformanekwork@proton.me" class="text-palwhite hover:animate-pulse hover:text-paldark">dformanekwork@proton.me</a></h2>
    
    </div>
</div>

<main>
<slot />
</main>
<style lang="postcss">
  /*:global(html) {
    background-color: theme(colors.);
    color: theme('colors.gray.800')
  }*/
</style>