<template>
  <UsersVue />
</template>

<script>
import UsersVue from '~/components/users/UsersVue.vue'
export default {
  name: 'Index',
  auth: true,
  components: { UsersVue },
  layout: 'DashboardVue'
}
</script>
