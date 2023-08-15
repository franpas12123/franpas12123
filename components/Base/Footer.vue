<template>
  <div>
    <p class="text-3xl">Footer</p>
    <p
      v-for="(attr, index) in attributions"
      :key="`attr-${index}`"
      v-html="attr"
    ></p>
  </div>
</template>

<script setup>
const attributions = [
  '<a href="https://www.freepik.com/free-vector/web-development-concept-with-programmer-ar_35496093.htm#query=developer&position=14&from_view=search&track=sph">Image by upklyak</a> on Freepik',
];
</script>

<style lang="scss" scoped></style>
