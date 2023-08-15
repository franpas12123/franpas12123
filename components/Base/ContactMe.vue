<template>
  <section id="contact-me" class="grid grid-cols-1 md:grid-cols-2">
    <div>
      <p class="text-4xl">Got a project in mind?</p>
    </div>
    <div>
      <div class="grid grid-cols-2">
        <div>
          <label for="name">Your name</label>
          <input type="text" name="name" id="name" />
        </div>
        <div>
          <label for="email">Your email</label>
          <input type="email" name="email" id="email" />
        </div>
      </div>
      <div class="grid grid-cols-1">
        <label for="message">Your message</label>
        <textarea name="message" id="1" cols="30" rows="10"></textarea>
      </div>
    </div>
  </section>
</template>

<script setup></script>

<style scoped></style>
