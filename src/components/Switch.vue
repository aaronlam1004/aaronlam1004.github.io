<template>
  <div>
    <label>
      <slot></slot>
      <span></span>
    </label>
  </div>
</template>

<style scoped>
@import '@/assets/base.css';

div {
  width: 4em;
  height: 1.5em;
  padding: 0em 1em;
}

label {
  position: absolute;
  width: 4em;
  height: 1.5em;
  background-color: var(--foreground-color);
  cursor: pointer;
  border-radius: 100px;
}

span {
  position: absolute;
  height: 1.3em;
  width: 1.3em;
  top: 0.1em;
  left: 0.1em;
  border-radius: 100px; 
  background-color: var(--background-color);
  transition: 0.4s;
}

:deep(input) {
  opacity: 0;
  width: 0;
  height: 0;
}

:deep(input:checked) + span {
  background-color: var(--background-color);
}

:deep(input:checked) + span {
  transform: translateX(2.4em);
}
</style>
