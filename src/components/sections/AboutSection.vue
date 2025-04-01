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
        I am a software engineer doing full-stack and embedded development.
      </p>
      <p>
        Some of my experience includes:
      </p>
      <ul>
        <li>Mobile Apps</li>
        <li>Web Apps</li>
        <li>Server Services</li>
        <li>Touch Applications</li>
        <li>Control Systems</li>
        <li>Embedded Drivers</li>
      </ul>
      <p>
        On my free time I like playing games with friend and am currently trying to learn new things.
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
  font-family: "DM Sans", sans-serif;
  width: 25%;
}

@media (max-width: 750px) {
  .content {
    font-size: 0.8em;
  }
  
  .content strong {
    font-size: 1.5em;
  }
}

@media (min-width: 750px) {
  .content {
    font-size: 1.25em;
  }
  
  .content strong {
    font-size: 1.5em;
  }
}
</style>
