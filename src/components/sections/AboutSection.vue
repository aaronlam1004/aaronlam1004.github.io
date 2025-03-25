<script setup lang="ts">
import Section from '@/components/Section.vue';
import profileImg from '@/assets/profile.jpg';
</script>

<template>
  <Section :image-src="profileImg">
    <template #title>About</template>
    <div class="content">
      <strong>Hello!</strong>
      <p>
        I am a software engineer that does full-stack and embedded work.
      </p>
      <p>
        In terms of experience, have developed/worked on:
      </p>
      <ul>
        <li>Mobile Apps</li>
        <li>Web Apps</li>
        <li>Server Services</li>
        <li>Touch Applications</li>
        <li>Control Systems</li>
        <li>Embedded Drivers</li>
        <li>Verification/Validation Scripts</li>
      </ul>
      <p>
        On my free time I like playing games with friend and am currently trying to learn video editing and music production.
      </p>
    </div>
  </Section>
</template>

<style scoped>
Section {
  display: flex;
  justify-content: space-evenly;
  flex-direction: row;
  flex-wrap: wrap;
}

.content {
  font-family: "Quicksand", sans-serif;
  width: 25%;
  font-size: 1.25em;
}

.content strong {
  font-size: 1.5em;
}
</style>
