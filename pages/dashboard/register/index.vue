<template>
  <RegisterVue />
</template>

<script>
import RegisterVue from '~/components/users/RegisterVue.vue'
export default {
  name: 'Index',
  auth: true,
  components: { RegisterVue },
  layout: 'DashboardVue'
}
</script>
