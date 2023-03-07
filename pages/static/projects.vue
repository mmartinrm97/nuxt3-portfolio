<template>
  <div class="flex w-full flex-col gap-8 lg:gap-12">
    <h1
      class="font-theme_bold text-xl text-head_text sm:text-3xl md:text-4xl md:leading-normal lg:text-6xl lg:leading-relaxed"
    >
      Projects<span class="text-link_text_hover">.</span>
    </h1>
    <p
      class="sg:leading-8 -mt-2 text-sm leading-relaxed md:text-base lg:text-lg"
    >
      Here are some projects I've worked on:
    </p>

    <hr class="h-[1px] border-0 bg-topbar bg-repeat" />

    <div class="flex flex-col items-center justify-center gap-28">
      <!-- Project -->
      <div class="flex flex-col items-center gap-8">
        <img
          alt="Project 1"
          src="~/assets/img/project-1.jpeg"
          class="w-full rounded-lg"
        />
        <div class="items-left flex flex-col gap-6 md:w-5/6">
          <span class="font-theme_bold text-2xl text-head_text">Project 1</span>
          <p class="text-sm lg:text-lg">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Totam at
            vitae eligendi tempora nemo id repellendus, minus consectetur libero
            a iure in? Maxime qui veritatis ullam velit nesciunt reprehenderit
            voluptatum?
          </p>
          <a
            class="font-theme_bold slg:text-base slg:px-6 slg:py-3 w-fit rounded-md border-[1px] border-link_border bg-btn_back px-2 py-2 text-sm text-btn_text transition-colors hover:bg-border_sm md:px-4"
            href="#"
            >Check Project
            <svg
              xmlns="http://www.w3.org/2000/svg"
              xmlns:xlink="http://www.w3.org/1999/xlink"
              aria-hidden="true"
              role="img"
              class="iconify iconify--ep inline text-xl"
              width="1em"
              height="1em"
              viewBox="0 0 1024 1024"
              style="color: rgb(234, 234, 234)"
            >
              <path
                fill="currentColor"
                d="M768 256H353.6a32 32 0 1 1 0-64H800a32 32 0 0 1 32 32v448a32 32 0 0 1-64 0V256z"
              ></path>
              <path
                fill="currentColor"
                d="M777.344 201.344a32 32 0 0 1 45.312 45.312l-544 544a32 32 0 0 1-45.312-45.312l544-544z"
              ></path></svg
          ></a>
        </div>
      </div>

      <!-- Project -->
      <div class="flex flex-col items-center gap-8">
        <img
          alt="Project 2"
          src="~/assets/img/project-2.jpeg"
          class="w-full rounded-lg"
        />
        <div class="items-left flex flex-col gap-6 md:w-5/6">
          <span class="font-theme_bold text-2xl text-head_text">Project 2</span>
          <p class="text-sm lg:text-lg">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Totam at
            vitae eligendi tempora nemo id repellendus, minus consectetur libero
            a iure in? Maxime qui veritatis ullam velit nesciunt reprehenderit
            voluptatum?
          </p>
          <a
            class="font-theme_bold slg:text-base slg:px-6 slg:py-3 w-fit rounded-md border-[1px] border-link_border bg-btn_back px-2 py-2 text-sm text-btn_text transition-colors hover:bg-border_sm md:px-4"
            href="#"
            >Check Project
            <svg
              xmlns="http://www.w3.org/2000/svg"
              xmlns:xlink="http://www.w3.org/1999/xlink"
              aria-hidden="true"
              role="img"
              class="iconify iconify--ep inline text-xl"
              width="1em"
              height="1em"
              viewBox="0 0 1024 1024"
              style="color: rgb(234, 234, 234)"
            >
              <path
                fill="currentColor"
                d="M768 256H353.6a32 32 0 1 1 0-64H800a32 32 0 0 1 32 32v448a32 32 0 0 1-64 0V256z"
              ></path>
              <path
                fill="currentColor"
                d="M777.344 201.344a32 32 0 0 1 45.312 45.312l-544 544a32 32 0 0 1-45.312-45.312l544-544z"
              ></path></svg
          ></a>
        </div>
      </div>
    </div>
  </div>
</template>
