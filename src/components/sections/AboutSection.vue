<script setup lang="ts">
import Section from '@/components/Section.vue';
</script>

<template>
  <Section>
    <template #title>About</template>
    <div class="content">
      <strong>Hello!</strong>
      <p>
        I am a software engineer with embedded, web, and mobile development experience.
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
