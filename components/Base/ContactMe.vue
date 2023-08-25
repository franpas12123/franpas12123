<template>
  <section
    id="contact-me"
    ref="contactMe"
    class="mt-20 grid grid-cols-1 px-5 sm:mt-0 sm:px-0 md:grid-cols-2"
  >
    <div class="z-10 lg:mx-12">
      <div class="mb-3 grid grid-cols-2 gap-5">
        <div class="input-label">
          <label for="name">Name</label>
          <input
            type="text"
            name="name"
            id="name"
            placeholder="Juan dela Cruz"
          />
        </div>
        <div class="input-label">
          <label for="email">Email</label>
          <input
            type="email"
            name="email"
            id="email"
            placeholder="juandelacruz@company.com"
          />
        </div>
      </div>
      <div class="input-label">
        <label for="message">Message</label>
        <textarea
          name="message"
          id="1"
          cols="30"
          rows="10"
          placeholder="Message me"
        ></textarea>
      </div>
    </div>
    <div class="">
      <!-- <p class="text-4xl">Got a project in mind?</p> -->
      <img
        class="deal mx-auto max-h-[450px]"
        src="img/partnership.gif"
        alt=""
      />
    </div>
  </section>
</template>

<script setup>
const form = reactive({
  name: null,
  email: null,
});
</script>

<style scoped>
input,
textarea {
  @apply rounded-xl text-black;
}
label {
  @apply pb-1 text-xl;
}
.input-label {
  @apply grid grid-cols-1;
}
.deal {
  /* @apply bg-gradient-to-b from-white via-white to-bg; */
}
#contact-me {
  min-height: 60vh !important;
  /* background-color: white; */
}
</style>
