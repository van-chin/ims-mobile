<script setup lang="ts">
const active = ref(0)
</script>

<template>
  <main p="16" text="gray-700 dark:gray-200">
    <RouterView />

    <van-tabbar v-model="active">
      <van-tabbar-item icon="home-o">
        首页
      </van-tabbar-item>
      <van-tabbar-item icon="search">
        工作区
      </van-tabbar-item>
      <van-tabbar-item>
        <template #icon>
          <van-icon name="add" size="3rem" />
        </template>
      </van-tabbar-item>
      <van-tabbar-item icon="friends-o">
        报表
      </van-tabbar-item>
      <van-tabbar-item icon="setting-o">
        个人中心
      </van-tabbar-item>
    </van-tabbar>
  </main>
</template>
