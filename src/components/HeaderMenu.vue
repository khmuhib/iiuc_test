<template>
  <div class="my-4">
    <nav class="p-2 bg-white shadow-xl md:flex md:items-center md:justify-center">
      <div class="flex justify-between items-center">
        <!-- <span class="text-2xl font-[Poppins] cursor-pointer">
          <img
            class="h-10 inline"
            src="https://tailwindcss.com/_next/static/media/social-square.b622e290e82093c36cca57092ffe494f.jpg"
          />
          tailwind
        </span> -->

        <span class="text-3xl cursor-pointer mx-2 md:hidden block">
          <ion-icon name="menu" onclick="Menu(this)"></ion-icon>
        </span>
      </div>

      <ul
        class="md:flex md:items-center md:justify-between z-[-1] md:z-auto md:static absolute bg-white w-full left-0 md:w-auto md:py-0 py-4 md:pl-0 pl-7 md:opacity-100 opacity-0 top-[-400px] transition-all ease-in duration-500"
      >
        <li class="mx-4 my-6 md:my-0">
          <a href="#" class="text-sm text-[#120D5E] hover:text-cyan-500 duration-500 font-bold">HOME</a>
        </li>
        <li class="mx-4 my-6 md:my-0">
          <a href="#" class="text-sm text-[#120D5E] hover:text-cyan-500 duration-500 font-bold">About IIUC</a>
        </li>
        <li class="mx-4 my-6 md:my-0">
          <a href="#" class="text-sm text-[#120D5E] hover:text-cyan-500 duration-500 font-bold">Administartion</a>
        </li>
        <li class="mx-4 my-6 md:my-0">
          <a href="#" class="text-sm text-[#120D5E] hover:text-cyan-500 duration-500 font-bold">Admission</a>
        </li>
        <li class="mx-4 my-6 md:my-0">
          <a href="#" class="text-sm text-[#120D5E] hover:text-cyan-500 duration-500 font-bold">Academic</a>
        </li>
        <li class="mx-4 my-6 md:my-0">
          <a href="#" class="text-sm text-[#120D5E] hover:text-cyan-500 duration-500 font-bold">Research & Publication</a>
        </li>
        <li class="mx-4 my-6 md:my-0">
          <a href="#" class="text-sm text-[#120D5E] hover:text-cyan-500 duration-500 font-bold">IQAC</a>
        </li>
        <li class="mx-4 my-6 md:my-0">
          <a href="#" class="text-sm text-[#120D5E] hover:text-cyan-500 duration-500 font-bold">Library</a>
        </li>
        <li class="mx-4 my-6 md:my-0">
          <a href="#" class="text-sm text-[#120D5E] hover:text-cyan-500 duration-500 font-bold">Conference</a>
        </li>
        <li class="mx-4 my-6 md:my-0">
          <a href="#" class="text-sm text-[#120D5E] hover:text-cyan-500 duration-500 font-bold">CGED</a>
        </li>
      </ul>
    </nav>
  </div>
</template>
<script>
export default {
  name: "HeaderMenu",
};

function Menu(e) {
  let list = document.querySelector("ul");
  e.name === "menu"
    ? ((e.name = "close"),
      list.classList.add("top-[80px]"),
      list.classList.add("opacity-100"))
    : ((e.name = "menu"),
      list.classList.remove("top-[80px]"),
      list.classList.remove("opacity-100"));
}
</script>

<style></style>
