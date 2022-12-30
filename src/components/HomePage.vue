<script setup lang="ts">
import { NLayout, NMessageProvider } from "naive-ui";
import HomeSider from "@/components/HomeSider.vue";
import HomeContent from "@/components/HomeContent.vue";
</script>

<template>
  <n-message-provider>
    <n-layout has-sider position="absolute" class="n-layout-b" style="">
      <HomeSider />
      <HomeContent />
    </n-layout>
  </n-message-provider>
</template>

<style scoped>
.n-layout-b {
  height: 100vh;
  background: radial-gradient(
      circle at 60% 90%,
      rgb(62, 127, 192),
      transparent 60%
    ),
    radial-gradient(
      circle at 20px 20px,
      rgba(60, 165, 214, 0.8),
      transparent 25%
    ),
    #2a3b57;
  border-radius: 20px;
  margin: 10px 10px;
  height: 96%;
}
</style>
