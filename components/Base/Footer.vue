<template>
  <section id="footer" class="min-h-5">
    <div class="grid grid-flow-row lg:mx-12 font-light text-sm text-center md:text-left">
      <span
        v-for="(attr, index) in attributions"
        :key="`attr-${index}`"
        v-html="attr"
      ></span>
    </div>
  </section>
</template>

<script setup>
const attributions = [
  '<a href="https://www.freepik.com/free-vector/web-development-concept-with-programmer-ar_35496093.htm#query=developer&position=14&from_view=search&track=sph">Image by upklyak</a> on Freepik',
  '<a href="https://storyset.com/people">People illustrations by Storyset</a>',
  '<a href="https://www.freepik.com/free-vector/software-development-backend-data-analysis-app-design-frontend-testing-flat-set-with-programmers-during-their-work-isolated-vector-illustration_40275497.htm#query=frontend&position=17&from_view=search&track=sph">Image by macrovector</a> on Freepik',
];
</script>

<style scoped>
#footer {
  min-height: auto !important;
}
</style>
