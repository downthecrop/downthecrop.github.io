<script>
import TeamCategory from "../components/TeamCategory.vue";
export default {
  components: {
    TeamCategory,
  },
  data() {
    return {
      config: {
        team: [{
          name:"Lytical",
          image: "https://github.com/LyticalApp/lyticalapp.github.io/blob/main/images/Lytical-social.png?raw=true",
          members:"bryce",
          description: "Open source League of Legends statistics and profile analytics tool for all regions including Garena & WeGame",
        },
        {
          name:"2009Scape Mobile",
          image: "https://i.imgur.com/o4nWDgF.png",
          members:"bryce",
          description: "Unoffical, unsupported, and unethical app to run 2009Scape on your Android device. Based on Pojav/Boardwalk.",
        },
        {
          name:"TTV-OLED",
          image: "https://i.imgur.com/Vq8kkC3.png",
          members:"bryce",
          description: "Load up a highly customizable Twitch chat with extension emotes (BTTV, FFZ, 7TV) on any device with a browser.",
        },
      ]
      },
    };
  },
};
</script>

<template>
  <div class="w-full md:h-full dark:bg-darkBackground">
    <div class="h-full mb-8 px-5 mx-auto py-48 max-w-page">
      <div class="max-w-6xl  mx-auto flex flex-row">
        <div class="w-full px-4 md:py-10 lg:w-6/12">
          <h2 class="md:hidden text-3xl font-extrabold leading-9 dark:text-white mb-5 flex flex-row md:justify-start justify-center">
            <img class="w-24 h-24 bg-black rounded-full dark:border-white" src="https://downthecrop.github.io/downthecrop.png" alt="" />
          </h2>
          <div class="mb-10 lg:mt-6 font-inter">
            <h2 class="mb-6 text-3xl font-bold leading-8 tracking-tight text-center dark:text-white sm:text-4xl md:text-left">
              downthecrop
              <br />
              <span class="inline-block pt-3 text-2xl text-pink-400">world famous video gamer and computer programmer</span>
            </h2>
            <p class="text-base text-center dark:text-white md:text-lg md:text-left">privacy enthusiast and technology philosopher. i make cool apps, youtube videos and stream on twitch.</p>
          </div>
          <div class="items-baseline pt-16 clients">
            <h6 class="flex items-center text-sm font-bold text-gray-500 uppercase font-inter text-body-color dark:text-white">Social Media</h6>
            <div class="flex items-center w-62">
              <div class="pt-3">
                <a target="_new" href="https://github.com/downthecrop"
                class="p-1 text-gray-500 text-4xl transition-colors duration-200 rounded-full focus:outline-none hover:text-pink-400 dark:hover:text-pink-400 dark:text-white md:ml-2">
                <font-awesome-icon icon="fa-brands fa-github" />
                </a>
                <a target="_new" href="https://twitter.com/downthecrop"
                class="p-1 text-gray-500 text-4xl transition-colors duration-200 rounded-full focus:outline-none hover:text-pink-400 dark:hover:text-pink-400 dark:text-white md:ml-2">
                <font-awesome-icon icon="fa-brands fa-twitter" />
                </a>
                <a target="_new" href="https://www.twitch.tv/downthecrop"
                class="p-1 text-gray-500 text-4xl transition-colors duration-200 rounded-full focus:outline-none hover:text-pink-400 dark:hover:text-pink-400 dark:text-white md:ml-2">
                <font-awesome-icon icon="fa-brands fa-twitch" />
                </a>
                <a target="_new" href="https://www.youtube.com/@downthecrop"
                class="p-1 text-gray-500 text-4xl transition-colors duration-200 rounded-full focus:outline-none hover:text-pink-400 dark:hover:text-pink-400 dark:text-white md:ml-2">
                <font-awesome-icon icon="fa-brands fa-youtube" />
                </a>
                <a target="_new" href="https://downthecrop.xyz/blog/"
                class="p-1 text-gray-500 text-4xl transition-colors duration-200 rounded-full focus:outline-none hover:text-pink-400 dark:hover:text-pink-400 dark:text-white md:ml-2">
                <font-awesome-icon icon="fa-brands fa-wordpress" />
                </a>
              </div>
            </div>
          </div>
        </div>
        <div class="z-10 justify-center hidden w-full px-4 py-10 lg:w-6/12 lg:flex">
          <img class="rounded-full scale-75 border-solid border-8 border-pink-300 top-0" src="https://downthecrop.github.io/downthecrop.png">
        </div>
      </div>
    </div>
  </div>
  <div class="w-full pt-10 pb-12 md:pb-32 lg:h-full dark:bg-darkBackground font-inter" id="about">
    <div class="px-8 mx-auto max-w-page">
      <div class="mx-auto max-w-5xl flex flex-col md:flex-row">
        <div class="flex flex-col w-full mr-8 md:w-1/3">
          <h2
            class="text-3xl font-extrabold leading-9 dark:text-white mb-4 flex flex-row md:justify-start justify-center">
            About Me
          </h2>
          <div class="mb-16 dark:text-white md:pr-16 pt-3 md:text-left text-center">
            <p>Hi I'm downthecrop. Experienced full stack developer with a passion for open source software. I travel the world, play video games, watch esports, and work on interesting projects.</p>
          </div>
        </div>
        <div class="w-full md:w-2/3 md:text-left text-center">
          <div class="mb-4">
            <h3 class="text-xl font-semibold text-pink-400">Programming Languages</h3>
          </div>
          <div class="mb-8 dark:text-white">
            <p>
              <a target="_new"
                class="p-1 text-gray-500 text-4xl transition-colors duration-200 rounded-full focus:outline-none hover:text-pink-400 dark:hover:text-pink-400 dark:text-white md:ml-2">
                <font-awesome-icon icon="fa-brands fa-vuejs" /> VueJS
                </a>
                <a target="_new"
                class="p-1 text-gray-500 text-4xl transition-colors duration-200 rounded-full focus:outline-none hover:text-pink-400 dark:hover:text-pink-400 dark:text-white md:ml-2">
                <font-awesome-icon icon="fa-brands fa-java" /> Java/Kotlin
                </a>
                <a target="_new"
                class="p-1 text-gray-500 text-4xl transition-colors duration-200 rounded-full focus:outline-none hover:text-pink-400 dark:hover:text-pink-400 dark:text-white md:ml-2">
                <font-awesome-icon icon="fa-brands fa-square-js" /> Vanilla JS
                </a>
            </p>
          </div>
          <div class="mb-4">
            <h3 class="text-xl font-semibold text-pink-400">Education</h3>
          </div>
          <div class="mb-8 dark:text-white">
            <p>
              Information Technology diploma with honors focused in Network Systems from Southern Alberta Institute of Technology.
            </p>
          </div>
        </div>
      </div>
      <div class="pt-10 max-w-6xl mx-auto w-full lg:h-full dark:bg-darkBackground font-roboto" id="team">
          <div class="px-8 mx-auto max-w-page">
            <div class="mb-20">
              <div class="mx-auto text-center md:max-w-xl lg:max-w-3xl">
                <h3 class="mb-6 text-3xl font-bold text-black dark:text-white" id="portfolio">Portfolio</h3>
                <p class="pb-2 mb-6 font-semibold text-pink-400 md:mb-12 md:pb-0">Amazing downthecrop software projects</p>
              </div>
              <div class="grid grid-cols-3 md:grid-cols-3 gap-6 text-center">
                <template v-for="(members, name) in config.team">
                  <TeamCategory :name="members.name" :image="members.image" :description="members.description" />
                </template>
              </div>
            </div>
          </div>
        </div>
        <div class="mx-auto text-center md:max-w-xl lg:max-w-3xl">
                <p class="pb-2 mb-6 font-semibold text-pink-300 md:mb-12 md:pb-0"><a href="/Projects">More projects...</a></p>
              </div>
      </div>
  </div>
</template>


