<template>
  <a :href="url">
    <div></div>
    <slot></slot>
  </a>
</template>

<script setup lang="ts">
const props = defineProps<{
  url: String
}>();
</script>

<style scoped>
a div {
  position: absolute;
  width: 2.25em;
  padding: 0.5em 0.5em;
  height: 2.25em;
  border-radius: 20px;
}

@keyframes rotate {
  from {
    transform: rotate(0);
  }
  to {
    transform: rotate(360deg);
  }
}

a:hover div {
  background: red;
  background: linear-gradient(
    90deg,
    hsla(248, 100%, 64%, 1) 0%,
    hsla(339, 100%, 55%, 1) 100%
  );
  animation: rotate 2s linear infinite;
}
</style>
