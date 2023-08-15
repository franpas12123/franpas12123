<template>
  <div class="grid grid-cols-2 p-3">
    <div class="my-auto">
      <nuxt-link to="/">
        <span class="text-xl">KZApps</span>
      </nuxt-link>
    </div>
    <nav>
      <ul class="flex justify-end lg:gap-7 gap-3">
        <li v-for="(img, index) in imgs" :key="index">
          <nuxt-link :to="{ path: img.link, hash: img.hash }">
            <img
              class="h-10 p-1 m-auto"
              :class="index + 1 === imgs.length ? 'pb-2' : ''"
              :src="`img/${img.src}`"
              :alt="img.src"
            />
          </nuxt-link>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script setup>
const imgs = reactive([
  { src: 'home.svg', link: '/' },
  { src: 'bullseye.svg', link: '/', hash: '#my-works' },
  { src: 'envelope.svg', link: '/', hash: '#contact-me' }
])
</script>

<style lang="scss" scoped></style>
