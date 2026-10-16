<script setup>
import { ref } from 'vue';

const theme = ref("dark");
const saved_theme = localStorage.getItem("theme");

if (saved_theme != null){
    theme.value = saved_theme;
}

function changeTheme(){
    if (theme.value == "dark"){
        document.documentElement.classList.add("dark");
        
    }
    else{
        document.documentElement.classList.remove("dark");
    }
    localStorage.setItem("theme",theme.value);
}

function toggleTheme(){
    theme.value = theme.value == "dark" ? "light" : "dark"
    console.log(theme.value)
    changeTheme()
}

changeTheme()


</script>

<template>
    <header class="sticky top-0 z-40 border-b border-neutral-200/80 bg-white/80 backdrop-blur-md transition-colors duration-300 dark:border-white/10 dark:bg-[#0a0a0b]/80">
    <div class="mx-auto flex h-16 max-w-7xl items-center justify-between px-6 lg:px-8">
      <a href="" class="flex items-center gap-2.5">
        <span class="flex h-9 w-9 items-center justify-center rounded-lg bg-accent-soft text-sm font-bold text-neutral-900">AH</span>
        <span class="text-lg font-semibold tracking-tight">amirhossein<span class="text-accent-soft">.dev</span></span>
      </a>

      <nav class="flex items-center gap-2 sm:gap-3">
        <button id="themeToggle" type="button" aria-label="Toggle theme" v-on:click="toggleTheme"
          class="cursor-pointer flex h-9 w-9 items-center justify-center rounded-lg border border-neutral-200 text-neutral-500 transition-colors hover:bg-neutral-100 hover:text-neutral-900 dark:border-white/10 dark:text-white/60 dark:hover:bg-white/5 dark:hover:text-white">
          <!-- Sun (visible in dark mode) -->
          <svg id="iconSun" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="hidden dark:inline h-5 w-5">
            <path stroke-linecap="round" stroke-linejoin="round" d="M12 3v2.25m6.364.386-1.591 1.591M21 12h-2.25m-.386 6.364-1.591-1.591M12 18.75V21m-4.773-4.227-1.591 1.591M5.25 12H3m4.227-4.773L5.636 5.636M15.75 12a3.75 3.75 0 1 1-7.5 0 3.75 3.75 0 0 1 7.5 0Z" />
          </svg>
          <!-- Moon (visible in light mode) -->
          <svg id="iconMoon" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="dark:hidden h-5 w-5">
            <path stroke-linecap="round" stroke-linejoin="round" d="M21.752 15.002A9.72 9.72 0 0 1 18 15.75c-5.385 0-9.75-4.365-9.75-9.75 0-1.33.266-2.597.748-3.752A9.753 9.753 0 0 0 3 11.25C3 16.635 7.365 21 12.75 21a9.753 9.753 0 0 0 9.002-5.998Z" />
          </svg>
        </button>

        <a href="./login.html" class="hidden rounded-lg px-3 py-2 text-sm font-medium text-neutral-600 transition-colors hover:text-neutral-900 sm:inline-block dark:text-white/70 dark:hover:text-white">Login</a>
        <a href="./signup.html" class="hidden rounded-lg bg-accent-soft px-4 py-2 text-sm font-semibold text-neutral-900 transition-colors hover:bg-accent sm:inline-block">Sign Up</a>
      </nav>
    </div>
  </header>
</template>