<template>
  <div>
    <!--Hero Section-->
    <div>
      <form action="" class="mt-20">
        <div
          class="w-full relative max-w-[860px] mx-auto px-5 pb-[138px] pt-24"
        >
          <div class="w-full mx-auto flex flex-col items-center justify-center">
            <h1 class="text-center w-full mx-auto heading-primary mb-3">
              The best Courses and Books on the
              <span class="text-orange">Laravel</span> ecosystem
            </h1>
            <p
              class="text-secoundery-color w-full text-lg text-center my-4 mb-10"
            >
              Find the right books and courses on the Laravel framework and
              related topics to suite your level of expertise. Know how good a
              course is through your peers review and share your own too.
            </p>

            <!--Search Form-->
            <div class="flex w-[700px] gap-x-6">
              <input
                type="search"
                name="keyword"
                placeholder="Enter keywords to search courses"
                class="w-4/5 bg-white h-12 border input-focus border-orange rounded-lg px-3.5 outline-none"
                required
              />
              <button type="submit" class="btn-primary w-1/5 text-white">
                Search
              </button>
            </div>
          </div>
          <!--hero icon-->
          <img
            src="https://laravel-courses.com/img/left-top-angle.png"
            alt="angle"
            class="absolute pointer-events-none top-[150px] -left-28"
          />
          <img
            src="https://laravel-courses.com/img/left-bottom-angle.png"
            alt="angle"
            class="absolute pointer-events-none top-[370px] -left-12"
          />
          <img
            src="https://laravel-courses.com/img/right-angle.png"
            alt="angle"
            class="absolute pointer-events-none top-[70px] -right-6"
          />
          <img
            src="https://laravel-courses.com/img/right-bottom-angle.png"
            alt="angle"
            class="absolute pointer-events-none top-[360px] -right-24"
          />
        </div>
      </form>
      <img
        src="https://laravel-courses.com/img/right-center-angle.png"
        alt="angle"
        class="w-auto h-auto object-contain absolute top-1/2 -translate-y-1/2 right-10 pointer-events-none"
      />
    </div>

    <!--Series Logo-->
    <div class="container mx-auto">
      <ul class="flex items-center flex-nowrap justify-between gap-y-7 gap-3">
        <li class="w-full lg:max-w-[165px]">
          <router-link
            to="/"
            class="bg-white border mx-auto border-orange box-shadow w-full h-12 md:h-16 rounded-lg flex items-center justify-center"
          >
            <img
              src="https://laravel-courses.com/storage/series/54e8baab-727e-4593-a78a-e0c22c569b61.png"
              alt="Laravel"
              class="w-20 md:w-auto h-auto object-contain"
            />
          </router-link>
        </li>
        <li class="w-full lg:max-w-[165px]">
          <router-link
            to="/"
            class="bg-white border mx-auto border-orange box-shadow w-full h-12 md:h-16 rounded-lg flex items-center justify-center"
          >
            <img
              src="https://laravel-courses.com/storage/series/54e8baab-727e-4593-a78a-e0c22c569b61.png"
              alt="Laravel"
              class="w-20 md:w-auto h-auto object-contain"
            />
          </router-link>
        </li>
        <li class="w-full lg:max-w-[165px]">
          <router-link
            to="/"
            class="bg-white border mx-auto border-orange box-shadow w-full h-12 md:h-16 rounded-lg flex items-center justify-center"
          >
            <img
              src="https://laravel-courses.com/storage/series/54e8baab-727e-4593-a78a-e0c22c569b61.png"
              alt="Laravel"
              class="w-20 md:w-auto h-auto object-contain"
            />
          </router-link>
        </li>
        <li class="w-full lg:max-w-[165px]">
          <router-link
            to="/"
            class="bg-white border mx-auto border-orange box-shadow w-full h-12 md:h-16 rounded-lg flex items-center justify-center"
          >
            <img
              src="https://laravel-courses.com/storage/series/54e8baab-727e-4593-a78a-e0c22c569b61.png"
              alt="Laravel"
              class="w-20 md:w-auto h-auto object-contain"
            />
          </router-link>
        </li>
        <li class="w-full lg:max-w-[165px]">
          <router-link
            to="/"
            class="bg-white border mx-auto border-orange box-shadow w-full h-12 md:h-16 rounded-lg flex items-center justify-center"
          >
            <img
              src="https://laravel-courses.com/storage/series/54e8baab-727e-4593-a78a-e0c22c569b61.png"
              alt="Laravel"
              class="w-20 md:w-auto h-auto object-contain"
            />
          </router-link>
        </li>
        <li class="w-full lg:max-w-[165px]">
          <router-link
            to="/"
            class="bg-white border mx-auto border-orange box-shadow w-full h-12 md:h-16 rounded-lg flex items-center justify-center"
          >
            <img
              src="https://laravel-courses.com/storage/series/54e8baab-727e-4593-a78a-e0c22c569b61.png"
              alt="Laravel"
              class="w-20 md:w-auto h-auto object-contain"
            />
          </router-link>
        </li>
      </ul>
    </div>
    <!--Feature Section-->
    <div class="container mx-auto mt-[140px]">
      <h1 class="heading-tertiory text-center mb-10 md:mb-16">
        Featured Courses
      </h1>
      <div class="w-full grid grid-cols-3 single-feature gap-10 mx-auto">
        <course-box
          v-for="(item, index) in courses"
          :course="item"
          :key="index"
        />
      </div>
      <div class="flex justify-center mt-12 mb-12">
        <router-link to="/courses">
          <button class="btn-primary text-white h-14 w-32">Browse all</button>
        </router-link>
      </div>
    </div>

    <!--Newsletter-->
    <div class="w-full bg-update bg-no-repeat bg-cover h-[400px] py-0">
      <div
        class="container mx-auto px-8 w-full flex flex-row justify-between items-center gap-5 h-full"
      >
        <div class="max-w-[579px] w-full">
          <h2 class="heading-secondary">Do not miss any updates</h2>
          <p class="mt-3.5 text-base-primary">
            We will be covering course reviews, comparison between the best
            courses, and will be sharing exclusive discounts with you on a
            monthly basis.
          </p>
          <div
            class="mt-6 md:mt-12 w-full flex flex-col sm:flex-row items-center gap-5"
          >
            <input
              wire:model="email"
              type="email"
              placeholder="Your email address"
              class="md:max-w-[385px] input-focus w-full h-14 bg-white border border-orange rounded-lg px-3.5 text-base-primary text-[#262626] placeholder:text-current outline-none"
            />
            <button
              wire:click="subscribe"
              class="bg-white w-full sm:w-[135px] shrink-0 h-14 rounded-lg flex justify-center items-center border border-orange text-lg-primary font-medium text-orange-100 bg-button-hover hover:text-white transition-all duration-300"
            >
              Subscribe
            </button>
          </div>
        </div>
        <div class="justify-center">
          <img
            src="https://laravel-courses.com/img/letter.png"
            alt="letter"
            class="w-auto h-auto object-contain"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";
import CourseBox from "../components/CourseBox.vue";

export default {
  components: { CourseBox },
  name: "HomePage",
  data() {
    return {
      courses: [],
      loading: true,
    };
  },
  mounted() {
    axios.get("https://laravel-courses.test/api/courses").then((response) => {
      // console.log(response.data);
      this.courses = response.data;
      this.loading = false;
    });
  },
};
</script>
