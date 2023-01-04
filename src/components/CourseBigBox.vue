<template>
  <li class="bg-white px-4 py-6 shadow rounded-sm">
    <div class="flex justify-center">
      <div class="min-w-fit mx-auto">
        <img
          class="inline-block w-10 rounded-full"
          src="https://laravel-courses.com/storage/series/d373d4a4-ee30-498b-99f6-259898fba344.png"
          alt="Laravel Logo"
        />
      </div>
      <div class="w-10/12">
        <div class="flex">
          <div class="flex-1 overflow-flex-wrap">
            <h2 class="text-xl font-bold text-gray-900 mb-1">
              <router-link
                :to="{ name: 'single-course' }"
                class="text-blue-500 hover:underline"
                >{{ course.name }}</router-link
              >
            </h2>
            <!-- <p>Duraton: {{ course.duration }}</p> -->
            <!-- <p>Platforms: {{ course.platform_id }}</p> -->
            <div class="flex items-center gap-3">
              <div class="flex items-center space-x-px">
                <svg
                  class="w-4 h-4 text-gray-300"
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 20 20"
                  fill="currentColor"
                >
                  <path
                    fill-rule="evenodd"
                    d="M10.868 2.884c-.321-.772-1.415-.772-1.736 0l-1.83 4.401-4.753.381c-.833.067-1.171 1.107-.536 1.651l3.62 3.102-1.106 4.637c-.194.813.691 1.456 1.405 1.02L10 15.591l4.069 2.485c.713.436 1.598-.207 1.404-1.02l-1.106-4.637 3.62-3.102c.635-.544.297-1.584-.536-1.65l-4.752-.382-1.831-4.401z"
                    clip-rule="evenodd"
                  ></path>
                </svg>
                <svg
                  class="w-4 h-4 text-gray-300"
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 20 20"
                  fill="currentColor"
                >
                  <path
                    fill-rule="evenodd"
                    d="M10.868 2.884c-.321-.772-1.415-.772-1.736 0l-1.83 4.401-4.753.381c-.833.067-1.171 1.107-.536 1.651l3.62 3.102-1.106 4.637c-.194.813.691 1.456 1.405 1.02L10 15.591l4.069 2.485c.713.436 1.598-.207 1.404-1.02l-1.106-4.637 3.62-3.102c.635-.544.297-1.584-.536-1.65l-4.752-.382-1.831-4.401z"
                    clip-rule="evenodd"
                  ></path>
                </svg>
                <svg
                  class="w-4 h-4 text-gray-300"
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 20 20"
                  fill="currentColor"
                >
                  <path
                    fill-rule="evenodd"
                    d="M10.868 2.884c-.321-.772-1.415-.772-1.736 0l-1.83 4.401-4.753.381c-.833.067-1.171 1.107-.536 1.651l3.62 3.102-1.106 4.637c-.194.813.691 1.456 1.405 1.02L10 15.591l4.069 2.485c.713.436 1.598-.207 1.404-1.02l-1.106-4.637 3.62-3.102c.635-.544.297-1.584-.536-1.65l-4.752-.382-1.831-4.401z"
                    clip-rule="evenodd"
                  ></path>
                </svg>
                <svg
                  class="w-4 h-4 text-gray-300"
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 20 20"
                  fill="currentColor"
                >
                  <path
                    fill-rule="evenodd"
                    d="M10.868 2.884c-.321-.772-1.415-.772-1.736 0l-1.83 4.401-4.753.381c-.833.067-1.171 1.107-.536 1.651l3.62 3.102-1.106 4.637c-.194.813.691 1.456 1.405 1.02L10 15.591l4.069 2.485c.713.436 1.598-.207 1.404-1.02l-1.106-4.637 3.62-3.102c.635-.544.297-1.584-.536-1.65l-4.752-.382-1.831-4.401z"
                    clip-rule="evenodd"
                  ></path>
                </svg>
                <svg
                  class="w-4 h-4 text-gray-300"
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 20 20"
                  fill="currentColor"
                >
                  <path
                    fill-rule="evenodd"
                    d="M10.868 2.884c-.321-.772-1.415-.772-1.736 0l-1.83 4.401-4.753.381c-.833.067-1.171 1.107-.536 1.651l3.62 3.102-1.106 4.637c-.194.813.691 1.456 1.405 1.02L10 15.591l4.069 2.485c.713.436 1.598-.207 1.404-1.02l-1.106-4.637 3.62-3.102c.635-.544.297-1.584-.536-1.65l-4.752-.382-1.831-4.401z"
                    clip-rule="evenodd"
                  ></path>
                </svg>
              </div>
              <span class="text-sm text-gray-500">0 Reviews</span>
            </div>
          </div>
        </div>
        <div class="mt-4 space-y-1 text-sm text-gray-700 line-clamp-5">
          <p>{{ course.description.substring(0, 300) }} ...</p>
        </div>
        <div class="mt-6">
          <div class="flex flex-col">
            <div class="flex space-x-0 gap-2 flex-wrap justify-items-start">
              <div class="inline-flex items-center gap-2 text-sm text-gray-500">
                <svg
                  class="w-6 h-6 text-gray-400 shrink-0"
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke-width="1.5"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="M3 13.125C3 12.504 3.504 12 4.125 12h2.25c.621 0 1.125.504 1.125 1.125v6.75C7.5 20.496 6.996 21 6.375 21h-2.25A1.125 1.125 0 013 19.875v-6.75zM9.75 8.625c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125v11.25c0 .621-.504 1.125-1.125 1.125h-2.25a1.125 1.125 0 01-1.125-1.125V8.625zM16.5 4.125c0-.621.504-1.125 1.125-1.125h2.25C20.496 3 21 3.504 21 4.125v15.75c0 .621-.504 1.125-1.125 1.125h-2.25a1.125 1.125 0 01-1.125-1.125V4.125z"
                  ></path>
                </svg>
                <span>Intermediate</span>
              </div>
              <div class="inline-flex items-center gap-2 text-sm text-gray-500">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke-width="1.5"
                  stroke="currentColor"
                  class="w-6 h-6 text-gray-400 shrink-0"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="M9 17.25v1.007a3 3 0 01-.879 2.122L7.5 21h9l-.621-.621A3 3 0 0115 18.257V17.25m6-12V15a2.25 2.25 0 01-2.25 2.25H5.25A2.25 2.25 0 013 15V5.25m18 0A2.25 2.25 0 0018.75 3H5.25A2.25 2.25 0 003 5.25m18 0V12a2.25 2.25 0 01-2.25 2.25H5.25A2.25 2.25 0 013 12V5.25"
                  />
                </svg>

                <span>{{ platformText[0].name }}</span>
              </div>
              <div class="inline-flex items-center gap-2 text-sm text-gray-500">
                <svg
                  class="w-6 h-6 text-gray-400 shrink-0"
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke-width="1.5"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="M12 6v6h4.5m4.5 0a9 9 0 11-18 0 9 9 0 0118 0z"
                  ></path>
                </svg>
                <span>{{ durationText }}</span>
              </div>
              <div class="inline-flex items-center gap-2 text-sm text-gray-500">
                <svg
                  class="w-6 h-6 text-gray-400 shrink-0"
                  xmlns="http://www.w3.org/2000/svg"
                  width="16"
                  height="16"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke-width="1.5"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="M12 6v12m-3-2.818l.879.659c1.171.879 3.07.879 4.242 0 1.172-.879 1.172-2.303 0-3.182C13.536 12.219 12.768 12 12 12c-.725 0-1.45-.22-2.003-.659-1.106-.879-1.106-2.303 0-3.182s2.9-.879 4.006 0l.415.33M21 12a9 9 0 11-18 0 9 9 0 0118 0z"
                  ></path>
                </svg>
                <span>${{ course.price }}.00</span>
              </div>
            </div>
          </div>
        </div>
        <div class="mt-6 flex justify-between space-x-8"></div>
      </div>
      <div class="flex w-1/12 overflow-hidden justify-end">
        <img
          class="inline-block h-8 w-8 rounded-full ring-2 ring-white"
          src="https://laravel-courses.com/storage/thumbnails/default/56/tp/g7t7058gcgwk00s48cwww.png?p=authors%2Fa489f89a-4866-4c10-961f-5fa6526d9709.png&amp;s=pd&amp;smartcrop=28x28"
          alt="Christoph Rumpel"
        />
      </div>
    </div>
  </li>
</template>

<script>
export default {
  name: "CourseBigBox",
  props: ["course", "platformText", "durationText"],
};
</script>

<style scoped></style>
