<template>
  <div>
    <nav class="dark:bg-darkBackground">
      <div class="px-5 mx-auto max-w-6xl mx-auto max-w-page">
        <div class="flex items-center justify-between h-20">
          <div class="flex items-center ">
            <a class="flex-shrink-0" href="/">
              <img class="w-10 h-10 rounded-full" :src="logo" alt="" />
            </a>
            <a class="flex-col justify-center font-rubik" href="/">
              <h1 class="px-4 text-xl font-bold text-pink-400 rounded-md dark:text-white" href="/#">
                downthecrop
              </h1>
              <h1 class="px-4 text-xs font-bold text-gray-500 uppercase rounded-md" href="/#">
                world famous video gamer
              </h1>
            </a>
          </div>
          <div class="hidden md:flex md:flex-row md:grow font-roboto">
            <div class="flex items-baseline ml-10 space-x-4">
              <a v-for="(i, idx) in paths" :key="idx"
                class="px-3 py-2 text-sm tracking-wide font-bold text-gray-500 transition-colors duration-200 uppercase rounded-md dark:text-white hover:font-bold hover:text-pink-400 dark:hover:text-pink-400"
                :href="i.path">
                {{ i.name }}
              </a>
            </div>
          </div>
          <div class="hidden lg:block md:block">
            <div class="flex items-center">
              <a href="https://github.com/downthecrop"
                class="p-1 text-gray-500 text-3xl transition-colors duration-200 rounded-full focus:outline-none hover:text-pink-400 dark:hover:text-pink-400 dark:text-white md:ml-2">
                <font-awesome-icon icon="fa-brands fa-github" />
              </a>
              <a href="https://twitter.com/downthecrop"
                class="p-1 text-gray-500 text-3xl transition-colors duration-200 rounded-full focus:outline-none hover:text-pink-400 dark:hover:text-pink-400 dark:text-white md:ml-2">
                <font-awesome-icon icon="fa-brands fa-twitter" />
              </a>
            </div>
          </div>
        </div>
        <Slide class="absolute top-0 right" v-if="showHambuger" right>
          <div class="block lg:hidden py-4 dark:bg-darkBackground">
            <div class="block items-baseline">
              <div v-for="(i, idx) in paths" :key="idx"
                class="px-3 py-2 text-sm tracking-wide font-bold text-gray-500 transition-colors duration-200 uppercase rounded-md dark:text-white hover:font-bold hover:text-pink-400 dark:hover:text-pink-400">
                <a :href="i.path">{{ i.name }}</a>
              </div>
              <a href="https://github.com/downthecrop"
                class="p-1 text-gray-500 text-3xl transition-colors duration-200 rounded-full focus:outline-none hover:text-pink-400 dark:hover:text-pink-400 dark:text-white md:ml-2">
                <font-awesome-icon icon="fa-brands fa-github" />
              </a>
              <a href="https://twitter.com/downthecrop"
                class="p-1 text-gray-500 text-3xl transition-colors duration-200 rounded-full focus:outline-none hover:text-pink-400 dark:hover:text-pink-400 dark:text-white md:ml-2">
                <font-awesome-icon icon="fa-brands fa-twitter" />
              </a>
            </div>
          </div>
        </Slide>
      </div>
    </nav>
  </div>
</template>

<script>
import { Slide } from 'vue3-burger-menu'  // import the CSS transitions you wish to use, in this case we are using `Slide`
export default {
  components: {
    Slide // Register your component
  },
  data() {
    return {
      logo: "https://downthecrop.github.io/downthecrop.png",
      showHambuger: false,
      windowWidth: window.innerWidth,
      paths: [
        {
          name: "Home",
          path: "/#",
        },
        {
          name: "About",
          path: "/#about",
        },
        {
          name: "Portfolio",
          path: "/#portfolio",
        },
      ],
    };
  },
  mounted() {
    this.$nextTick(() => {
      window.addEventListener('resize', this.onResize);
    })
    this.showHambuger = this.windowWidth <= 764
  },

  beforeDestroy() {
    window.removeEventListener('resize', this.onResize);
  },

  methods: {
    onResize() {
      this.windowWidth = window.innerWidth
      this.showHambuger = this.windowWidth <= 764
    }
  }
}
</script>

<style>
.right {
  z-index: 999;
  right: 50px;
}
</style>