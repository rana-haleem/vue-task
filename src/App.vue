<template>
  <Header />
  <VideoBanner/>
  <Notifications/>
</template>

<script>
import Header from '@/components/Header.vue'
import VideoBanner from '@/components/VideoBanner.vue'
import Notifications from '@/components/Notifications.vue'
export default {
  name: 'App',
  components: {
    Header,
    VideoBanner,
    Notifications
  }
}
</script>

<style>
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
</style>
