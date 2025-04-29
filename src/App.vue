<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import { Toaster } from '@/components/ui/sonner'
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/projects">プロジェクト設定</RouterLink>
        <RouterLink to="/login">Login</RouterLink>
        <RouterLink to="/user">ユーザー管理</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
  <Toaster />
</template>

<style scoped></style>
