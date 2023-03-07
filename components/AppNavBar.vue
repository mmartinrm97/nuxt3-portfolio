<template>
  <Teleport to="body">
    <!-- NavBar -->
    <nav
      class="fixed flex w-full items-center justify-between border-b-[1px] border-border_sm bg-navbar_back px-3 py-3 backdrop-blur-sm sm:top-0 sm:bottom-auto sm:px-6 lg:py-4"
    >
      <div class="absolute top-0 left-0 h-[1px] w-full bg-topbar lg:h-1"></div>
      <a
        aria-current="page"
        href="/"
        class="router-link-active router-link-exact-active select-none text-3xl font-normal lg:text-4xl"
      >
        My Portfolio
      </a>
      <div class="flex items-center gap-1 text-sm sm:gap-2">
        <NuxtLink to="/">
          <span
            class="rounded-md px-3 py-1 pb-2 transition-all hover:bg-action_back sm:px-6 sm:py-2 lg:text-sm"
          >
            Home
          </span>
        </NuxtLink>
        <NuxtLink to="/projects">
          <span
            class="rounded-md px-3 py-1 pb-2 transition-all hover:bg-action_back sm:px-6 sm:py-2 lg:text-sm"
          >
            Projects
          </span>
        </NuxtLink>
        <NuxtLink to="/about">
          <span
            class="rounded-md px-3 py-1 pb-2 transition-all hover:bg-action_back sm:px-6 sm:py-2 lg:text-sm"
          >
            About
          </span>
        </NuxtLink>
      </div>
    </nav>
  </Teleport>
</template>
