<template>
  <div class="w-full md:w-2/3 md:text-left text-center mx-auto pt-20">
    <div v-for="project of projects">
      <div class="mb-4">
        <a target="_new" class="hover:underline" :href="project.url">
        <h3 class="text-xl hover:underline font-semibold text-pink-400">{{project.name}}</h3>
        </a>
      </div>
      <div class="mb-8 dark:text-white">
        <p>
          {{project.description}}
          <br>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
/*
  TODO: Add sorting options based on date created and alphabetical order
*/

export default {
data() {
    return {
      projects: [
        {
          name:"2009Scape-macOS-HD",
          url: "https://github.com/downthecrop/2009Scape-macOS-HD",
          description: "Exactly what it sounds like. Saradomin Launcher in a WineskinWrapper for HD/OpenGL on macOS.", 
        },
        {
          name:"GIF Optimizer",
          url: "https://github.com/downthecrop/GIF-Optimizer",
          description: "Fast and customizable GIF compression! Electron app wrapper for FFMPEG.", 
        },
        {
          name:"Minimal New Tab Extension",
          url: "https://github.com/downthecrop/minimal-new-tab",
          description: "I really don't like google doodles on my newtab pages. Unfortunatly due to some chrome premission settings the chrome://newtab page is unable to be hooked. And thus we can't just block doodle requests. This is an all in one drop in replacement for the Chrome new tab.", 
        },
        {
          name:"Minimal Scrollbar",
          url: "https://github.com/downthecrop/minimal-new-tab",
          description: "Chrome improvement project. Makes the overflow scrollbar on pages consistent and minimal. All CSS. NO JavaScript. Featured by the Chromestore!", 
        },
        {
          name:"RuneLite But You Can Save Your Password (BYCSYP)",
          url: "https://github.com/downthecrop/runelite-but-you-can-save-your-password",
          description: "RuneLite is a free, open source OldSchool RuneScape client... that didn't let you save your password and now you can!", 
        },
        {
          name:"checkra1n TWRP",
          url: "https://github.com/downthecrop/checkra1n-twrp",
          description: "Automate TWRP commands to launch checkra1n on arm/arm64 Android", 
        },
        {
          name:"checkra1n-linux minimal Live USB",
          url: "https://github.com/downthecrop/checkra1n-linux",
          description: "Portable minimal boot environment for use with checkra1n. This respin of Minimal Linux Live provides everything you need to run checkra1n for iOS/tvOS in under 70MB.", 
        },
        {
          name:"OPGG Clone for WeGame/Tencent Chinese/CN Servers",
          url: "https://github.com/downthecrop/wegame-tencent-china-opgg",
          description: "Pregame lobby Multisearch, Game Details and Profile Statistics from WeGame/Tencent League of Legends LoL API", 
        },
        {
          name:"Better Better Destiny.gg (BBDGG)",
          url: "https://github.com/downthecrop/bbdgg",
          description: "An unofficial browser extension to add unofficial functionality to the destiny.gg chat.", 
        },
        {
          name:"OSRS Jad Simulator",
          url: "https://github.com/downthecrop/JS-OSRS-Jad-Simulator",
          description: "Asset swapped RS3 Jad Simulator for Old School Runescape", 
        },
        {
          name:"Adobe Photoshop CS2 Patcher",
          url: "https://github.com/downthecrop/CS2-Patcher",
          description: "Asset swapped RS3 Jad Simulator for Old School Runescape", 
        },
        {
          name:"Audio Remuxer",
          url: "https://github.com/downthecrop/audio-remuxer",
          description: "FFmpeg audio channel remuxer for use with multitrack recordings from OBS", 
        },
        {
          name:"TwitchVOD",
          url: "https://github.com/downthecrop/TwitchVOD",
          description: "Keep your past broadcasts safe from being muted. Private remote VOD recordings.", 
        },
        {
          name:"2009Scape Drop Table Tool",
          url: "https://github.com/2009scape/2009scape.github.io/pull/173",
          description: "Search which NPCs drop which items and their rarities.", 
        },

    ]
    };
  }
}
</script>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
