<template>
  <section id="my-services" class="px-3">
    <p class="section-title">My Services</p>
    <div class="mt-10 grid grid-cols-1 gap-5 md:grid-cols-2 lg:grid-cols-3">
      <!-- <div v-for="(tech, index) in techs" :key="index">
        <a class="text-center" :href="tech.link">
          <img class="mx-auto h-10 w-10" :src="tech.logo" alt="" />
        </a>
      </div> -->
      <BaseCard
        v-for="(service, index) in services"
        :key="`service-${index}`"
        :img-src="service.imgSrc"
        :title="service.name"
        class="m-5 mx-auto max-w-[350px]"
        description=""
        :light="true"
        :shadow="true"
      />
    </div>
  </section>
</template>

<script setup>
const services = [
  {
    name: "Frontend Development",
    imgSrc: "frontend.png",
  },
  {
    name: "Backend Development",
    imgSrc: "backend.png",
  },
  {
    name: "Responsive Design",
    imgSrc: "responsive.png",
  },
  {
    name: "Testing",
    imgSrc: "testing.png",
  },
  {
    name: "Bug Fixing",
    imgSrc: "bugfixing.png",
  },
  {
    name: "Deployment",
    imgSrc: "deployment.png",
  },
];
</script>

<style scoped></style>
