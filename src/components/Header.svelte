<script>
  import logo from "../resources/images/logo.jpg"
  import { goto } from '$app/navigation'
</script>

<div class="flex bg-gray-50 w-full">
  <img src={logo} on:click={()=>goto("/")} alt="logo" width={70} height={20} />

  <span class="justify-center items-center relative group md:flex hidden">
    <button class=" hover:text-gray-400 md:ml-12 ml-2"> Who are we </button>
    <div
      class="absolute left-0 hidden space-y-2 mt-48 bg-white text-black shadow-lg group-hover:block rounded-md w-48 p-2"
    >
      <a href="#" class="block md:px-4 md:py-2 px-2 py-1 hover:bg-gray-100">About us</a>
      <a href="#" class="block md:px-4 md:py-2 px-2 py-1 hover:bg-gray-100">Partner with us</a>
      <a href="#" class="block md:px-4 md:py-2 px-2 py-1 hover:bg-gray-100">Resources</a>
    </div>
  </span>
  <span class="justify-center items-center md:ml-20 ml-2 md:flex hidden"
    ><a href="#" class="block md:px-4 md:py-2 px-2 py-1 hover:bg-gray-100">What we do</a></span
  >
  <!-- <span class="flex justify-center items-center relative group md:ml-20 ml-2">
    <button class=" hover:text-gray-400"> Services </button>
    <div
      class="absolute left-0 hidden space-y-2 mt-48 bg-white text-black shadow-lg group-hover:block rounded-md w-48 p-2"
    >
      <a href="#" class="block md:px-4 md:py-2 px-2 py-1 hover:bg-gray-100">Web Development</a>
      <a href="#" class="block md:px-4 md:py-2 px-2 py-1 hover:bg-gray-100">App Development</a>
      <a href="#" class="block md:px-4 md:py-2 px-2 py-1 hover:bg-gray-100">SEO Optimization</a>
    </div>
  </span>
  <span class="justify-center items-center relative group md:ml-20 ml-2 md:flex hidden">
    <button class=" hover:text-gray-400"> Technologies </button>
    <div
      class="absolute left-0 hidden space-y-2 mt-48 bg-white text-black shadow-lg group-hover:block rounded-md w-48 p-2"
    >
      <a href="#" class="block md:px-4 md:py-2 px-2 py-1 hover:bg-gray-100">Web Development</a>
      <a href="#" class="block md:px-4 md:py-2 px-2 py-1 hover:bg-gray-100">App Development</a>
      <a href="#" class="block md:px-4 md:py-2 px-2 py-1 hover:bg-gray-100">SEO Optimization</a>
    </div>
  </span>
  <span class="flex justify-center items-center relative group md:ml-20 ml-2">
    <button class=" hover:text-gray-400"> Insights </button>
    <div
      class="absolute left-0 hidden space-y-2 mt-48 bg-white text-black shadow-lg group-hover:block rounded-md w-48 p-2"
    >
      <a href="#" class="block md:px-4 md:py-2 px-2 py-1 hover:bg-gray-100">Web Development</a>
      <a href="#" class="block md:px-4 md:py-2 px-2 py-1 hover:bg-gray-100">App Development</a>
      <a href="#" class="block md:px-4 md:py-2 px-2 py-1 hover:bg-gray-100">SEO Optimization</a>
    </div>
  </span> -->
  <span class="flex justify-center items-center md:ml-20 ml-2"
    ><a href="#" class="block md:px-4 md:py-2 px-2 py-1 hover:bg-gray-100">Industries</a></span
  >
  <span class="flex justify-center items-center md:ml-20 ml-2"
    ><a href="/contact-us" class="block md:px-4 md:py-2 px-2 py-1 hover:bg-gray-100">Contact us</a></span
  >
</div>
