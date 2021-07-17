<template>
  <Header />
  <VideoBanner/>
  <Notifications/>
  <Next/>
</template>

<script>
import Header from '@/components/Header.vue'
import VideoBanner from '@/components/VideoBanner.vue'
import Notifications from '@/components/Notifications.vue'
import Next from '@/components/Next.vue'
export default {
  name: 'App',
  components: {
    Header,
    VideoBanner,
    Notifications,
    Next
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
