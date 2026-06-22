<template>
  <a :href="url" target="_blank">
    <div></div>
    <slot></slot>
  </a>
</template>

<script setup lang="ts">
const props = defineProps<{
  url: string
}>();
</script>

<style scoped>
@keyframes rotate {
  from {
    transform: rotate(0);
  }
  to {
    transform: rotate(360deg);
  }
}

a div {
  position: absolute;
  width: 2.25em;
  height: 2.25em;
  padding: 0.5em 0.5em;
  border-radius: 20px;
  animation: rotate 2s linear infinite;
}

a:hover div {
  background: var(--foreground-color); 
}

</style>
