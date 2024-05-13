<script setup lang="ts">
const users = ['usera', 'userb', 'userc']
const posts = [
  {
    title: 'Post',
    user: {
      name: 'user a'
    }
  },
  {
    title: 'Post',
    user: {
      name: 'user b'
    }
  },
  {
    title: 'Post',
    user: {
      name: 'user c'
    }
  }
]
</script>
<template>
  <div v-for="(user, index) in users" :key="index">
    {{ user }}
  </div>
  <div v-for="(post, index) in posts" :key="index">
    title ={{ post.title }} creator ={{ post.user.name }}
  </div>
</template>

<style scoped></style>
