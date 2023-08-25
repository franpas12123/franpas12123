<template>
  <section id="techs-used" class="mt-28 px-3">
    <p class="section-title">Techs Used</p>
    <div class="mt-20 grid grid-cols-3 gap-10 sm:grid-cols-5 md:grid-cols-6">
      <div v-for="(tech, index) in techs" :key="index">
        <a class="text-center" :href="tech.link">
          <img
            class="m-auto h-20 w-20 rounded-xl p-3 shadow shadow-cyan-700/50 hover:bg-cyan-800 hover:shadow-cyan-500/50"
            :src="tech.logo"
            alt=""
          />
        </a>
      </div>
    </div>
  </section>
</template>

<script setup>
const techs = reactive({
  nuxt: {
    link: "https://nuxtjs.org/",
    logo: "img/nuxtjs.svg",
    name: "NuxtJS",
  },
  vue: {
    link: "https://vuejs.org/",
    logo: "img/vuejs.svg",
    name: "VueJS",
  },
  tailwind: {
    link: "https://tailwindcss.com/",
    logo: "img/tailwindcss.svg",
    name: "TailwindCSS",
  },
  html: {
    link: "https://developer.mozilla.org/en-US/docs/Web/HTML",
    logo: "img/html5.svg",
    name: "HTML",
  },
  css: {
    link: "https://developer.mozilla.org/en-US/docs/Web/CSS",
    logo: "img/css3.svg",
    name: "CSS",
  },
  bootstrap: {
    link: "https://getbootstrap.com/",
    logo: "img/bootstrap.svg",
    name: "Bootstrap",
  },
  js: {
    link: "https://developer.mozilla.org/en-US/docs/Web/JavaScript",
    logo: "img/javascript.svg",
    name: "JavaScript",
  },
  typescript: {
    link: "https://www.typescriptlang.org/",
    logo: "img/typescript.svg",
    name: "TypeScript",
  },
  vite: {
    link: "https://vitejs.dev/",
    logo: "img/vitejs.svg",
    name: "ViteJS",
  },
  supabase: {
    link: "https://https://supabase.com/",
    logo: "img/supabase.svg",
    name: "Supabase",
  },
  firebase: {
    link: "https://firebase.google.com/",
    logo: "img/firebase.svg",
    name: "Firebase",
  },
  ionic: {
    link: "https://ionicframework.com/docs/vue/overview",
    logo: "img/ionic.svg",
    name: "Ionic Vue",
  },
  netlify: {
    link: "https://www.netlify.com/",
    logo: "img/netlify.svg",
    name: "Netlify",
  },
  github: {
    link: "https://www.github.com",
    logo: "img/github.svg",
    name: "GitHub",
  },
  bitbucket: {
    link: "https://bitbucket.org/",
    logo: "img/bitbucket.svg",
    name: "Bitbucket",
  },
  slack: {
    link: "https://slack.com/",
    logo: "img/slack.svg",
    name: "Slack",
  },
  discord: {
    link: "https://discord.com/",
    logo: "img/discord.svg",
    name: "Discord",
  },
  jira: {
    link: "https://jira.atlassian.com/",
    logo: "img/jira.svg",
    name: "Jira",
  },
  trello: {
    link: "https://trello.com/",
    logo: "img/trello.svg",
    name: "Trello",
  },
  notion: {
    link: "https://www.notion.so/",
    logo: "img/notion.svg",
    name: "Notion",
  },
});
</script>

<style scoped>
#techs-used {
  min-height: 85vh !important;
}
</style>
