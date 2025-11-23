<template>
    <div class="d-flex flex-column profile-content w-100 gap-4">
        <div class="d-flex header-profile justify-content-between">
          <change-theme />
        </div>
      <div class="d-flex body-profile">
        <img src="@/public/image/pouria.jpg" alt="">
      </div>
      <div class="d-flex flex-column footer-profile justify-content-center">
        <div class="d-flex flex-column justify-content-center align-items-center">
          <h2>Pouria Rahimy</h2>
          <p>Software Engineer</p>
        </div>
        <div class="d-flex social-media">
          <span v-for="(item) in socialMedia" :key="item.id" class="circle-social">
            <Link :href="item.link">
              <img :src="item.icon" alt="LinkedIn" />
            </Link>
          </span>
        </div>
      </div>
      <div class="d-flex link w-100">
        <button class="w-100 p-2 ">Download CV</button>
      </div>
    </div>
</template>

<script setup lang="ts">

import ChangeTheme from "~/components/changeTheme.vue";

const socialMedia = [
  {id: 1, title: "LinkedIn", icon: '@/public/image/linked.jpg', link: ''},
  {id: 2, title: "GitHub", icon: '@/public/image/github.png', link: ''},
  {id: 2, title: "Instagram", icon: '@/public/image/instagram.svg', link: ''},
  {id: 2, title: "Telegram", icon: '@/public/image/telegram.svg', link: ''}
]
</script>

<style scoped>

</style>