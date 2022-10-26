<template>
  <v-app id="inspire" class="background">
    <Drawer />
    <v-main>
      <nuxt />
    </v-main>
  </v-app>
</template>

<script>
import Drawer from '~/components/dashboard/Drawer.vue'
export default {
  components: {
    Drawer
  }
}
</script>

<style scoped>
.background {
  background-color: #354551;
}
</style>
