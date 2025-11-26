<template>
  <div class="layout">
    <div class="header-slider-wrapper">
      <Slider />
      <header class="header-mind-nest">
        <div class="flex sub-header">
          <toolbar />
        </div>
        <div class="flex header-navbar">
          <navbar />
        </div>
      </header>
    </div>

    <main class="container-fluid">
      <slot />
    </main>

    <footer>footer</footer>
  </div>
</template>

<script setup lang="ts">
import toolbar from '~/components/header/toolbar.vue'
import navbar from '~/components/header/navbar.vue'
import Slider from '@/components/home/slider.vue'
</script>

<style scoped>
.header-slider-wrapper {
  position: relative;
}

.header-mind-nest {
  position: absolute;
  width: 100%;
  top: 0;
  left: 0;
  z-index: 10;
}
.header-navbar{
  background-color: white;
  width: 70%;
  display: flex;
  margin: 0 auto;
}

header + Slider {
  z-index: 1;
}
</style>
