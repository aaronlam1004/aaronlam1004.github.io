<template>
  <section>
    <h1><slot name="title"></slot></h1>
    <slot></slot>
  </section>
</template>

<style scoped>
h1 {
  margin: 0;
  width: 100%;
  font-family: "Poetsen One", sans-serif;
  font-size: 4em;
  text-align: center;
}

section {
  width: 100%;
  height: 100%;
  box-sizing: border-box;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
</style>