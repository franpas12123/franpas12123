<template>
  <div
    class="card-container container rounded-xl p-5"
    :class="[light ? 'bg-[#226faa7d]' : 'bg-[#171c22]', { shadow }]"
  >
    <img
      :src="`img/my-services/${props.imgSrc}`"
      :class="imgClass"
      class="max-w-[300px] rounded-xl"
      alt=""
    />
    <p class="title text-center text-2xl font-light">
      {{ title }}
    </p>
    <p v-if="description" class="description mt-5 text-center font-light">
      {{ description }}
    </p>
  </div>
</template>

<script lang="ts" setup>
const props = defineProps({
  light: {
    type: Boolean,
    default: false,
  },
  shadow: {
    type: Boolean,
    default: false,
  },
  imgSrc: {
    type: String,
    default: "frontend.png",
  },
  imgClass: {
    type: String,
    default: "mx-auto",
  },
  title: {
    type: String,
    default: "Web Developer",
  },
  description: {
    type: String,
    default:
      "Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum earum quia maxime minus pariatur accusamus eos aspernatur culpa atque est debitis necessitatibus.",
  },
});
</script>

<style scoped>
.card-container {
  /* background-color: rgb(59, 59, 59); */
}
</style>
