<template>
  <div class="d-flex flex-column gap-4">
    <div class="d-flex flex-column">
      <toolbar />
      <div class="d-flex">
        <header class="header-mind-nest d-flex flex-column mx-auto">
          <navbar />
        </header>
      </div>
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
</script>

<style scoped>

</style>