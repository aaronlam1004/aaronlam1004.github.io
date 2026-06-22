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
  width: 3em;
  height: 1.5em;
  padding: 0em 1em;
}

label {
  position: absolute;
  width: 3em;
  height: 1.5em;
  background-color: var(--foreground-color);
  cursor: pointer;
  border-radius: 34px;
}

span {
  position: absolute;
  height: 1.3em;
  width: 1.3em;
  top: 0.1em;
  left: 0.1em;
  border-radius: 34px; 
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
  transform: translateX(1.45em);
  top: 0.225em;
  width: 1.1em;
  height: 1.05em;
}
</style>
