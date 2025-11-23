<template>
  <div class="bg-[var(--bg-body)] main-page">
      <div class="d-flex w-100">
        <div class="d-flex w-30">
          <profile-content />
        </div>
        <div class="d-flex w-70">
          body page
        </div>
      </div>
  </div>
</template>

<script setup lang="ts">

import ProfileContent from "~/components/homePage/profileContent.vue";
</script>

<style scoped>

</style>