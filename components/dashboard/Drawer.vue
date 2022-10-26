<template>
  <v-navigation-drawer absolute permanent left app color="#10445A">
    <template #prepend>
      <v-list-item two-line>
        <v-list-item-avatar>
          <img src="https://randomuser.me/api/portraits/men/65.jpg">
        </v-list-item-avatar>

        <v-list-item-content>
          <v-list-item-title>Angel Ramírez</v-list-item-title>
          <v-list-item-subtitle>Logged In</v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>
    </template>

    <v-divider />

    <v-list dense>
      <v-list-item v-for="item in items" :key="item.title" :to="item.path">
        <v-list-item-icon>
          <v-icon>{{ item.icon }}</v-icon>
        </v-list-item-icon>

        <v-list-item-content>
          <v-list-item-title>{{ item.title }}</v-list-item-title>
        </v-list-item-content>
      </v-list-item>
    </v-list>
  </v-navigation-drawer>
</template>

<script>
export default {
  data () {
    return {
      items: [
        {
          title: 'Registo',
          icon: 'mdi-account-plus-outline',
          path: '/dashboard/register'
        },
        {
          title: 'Usuarios',
          icon: 'mdi-account-group-outline',
          path: '/dashboard/users'
        }
      ]
    }
  }
}
</script>
