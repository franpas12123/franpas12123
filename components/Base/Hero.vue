<template>
  <section id="hero" class="mx-3 h-screen md:mt-10 md:-mb-10">
    <div class="grid gap-5 sm:h-2/3 sm:grid-cols-5">
      <div
        class="order-last my-auto grid content-end sm:order-1 sm:col-span-2 sm:pt-10"
      >
        <p
          class="mb-2 text-center text-5xl font-bold text-cyan-400 sm:text-end"
        >
          {{ name }}
        </p>
        <p class="text-center text-2xl font-light uppercase sm:text-end">
          {{ position }}
        </p>
        <p class="mt-5 text-center font-extralight sm:text-end">
          {{ description }}
        </p>
        <div class="mx-auto mt-5 sm:ml-auto sm:mr-0">
          <button
            type="button"
            class="rounded-xl bg-cyan-500 p-3 px-5 text-xl font-medium text-white shadow"
            @click="handleClick"
          >
            {{ ctaText }}
          </button>
        </div>
      </div>
      <div class="order-1 my-auto sm:order-last sm:col-span-3">
        <img class="hero mx-auto sm:mr-auto" src="img/hero.png" alt="hero" />
      </div>
    </div>
  </section>
</template>

<script lang="ts" setup>
import { ref, onMounted } from "vue";
const name = "Frances Pasulohan";
const position = "full-stack developer";
const description =
  "Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis, eveniet quo ipsam magnam eius explicabo expedita quis natus aperiam?";
const ctaText = "Contact Me";

onMounted(() => {
  // contactMe.scrollIntoView({ behavior: "smooth" });
});
const handleClick = () => {
  window.scrollTo(0, 9999);
  // console.log("ref", ref.);
  // const el =
  // ref.scrollIntoView({ behavior: "smooth" });
};
</script>

<style scoped></style>
