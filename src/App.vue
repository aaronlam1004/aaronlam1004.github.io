<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import Switch from '@/components/Switch.vue';
</script>

<template>
  <header>
    <p class="sprite"></p>
    <Switch>
      <input @change="toggleTheme" type="checkbox"/>
    </Switch>
  </header>
  <RouterView/>
</template>

<style scoped>
@import '@/assets/base.css';

header {
  display: flex;
  flex-direction: row-reverse;
  align-items: center;
}

.sprite {
  width: 5em;
  height: 4em;
  background-image: var(--sprite);
  background-size: 4em;
  background-repeat: no-repeat;
  filter: drop-shadow(1.5px 1.5px 1.5px var(--sprite-bg-color));
}
</style>

<script lang="ts">
// Themes
const useMew = Math.random() >= 0.8;

enum Theme {
  Light = "light-theme",
  Dark  = "dark-theme"
}

function setTheme(theme: Theme) : void {
  localStorage.setItem("user-theme", theme);
  document.documentElement.className = theme;
  if (useMew) {
    document.documentElement.className += " mew";
  }
}

function toggleTheme() : void {
  const activeTheme = localStorage.getItem("user-theme");
  if (activeTheme == Theme.Light) {
    setTheme(Theme.Dark);
  } else {
    setTheme(Theme.Light);
  }
}

function isNight() : bool {
  const date = new Date();
  const hours = date.getHours();
  return (hours < 6) || (hours >= 18);
}

// Export
export default {
  mounted() {
    if (isNight()) {
      setTheme(Theme.Dark);
    } else {
      setTheme(Theme.Light);
    }
  }
}
</script>
