<template>
  <div>
    <v-navigation-drawer v-model="drawer">
      <v-list>
        <v-list-item prepend-avatar="https://randomuser.me/api/portraits/women/85.jpg" title="Sandra Adams"
          subtitle="sandra_a88@gmailcom"></v-list-item>
      </v-list>

      <v-divider></v-divider>

      <v-list density="compact" nav>
        <v-list-item prepend-icon="mdi-view-dashboard" title="Dashboard" value="dashboard"></v-list-item>
        <v-list-item prepend-icon="mdi-crowd" title="Audience" value="audience"></v-list-item>
        <v-list-item prepend-icon="mdi-calendar" title="Events" value="events"></v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar>

      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>

      <v-app-bar-title>VEC App</v-app-bar-title>
    </v-app-bar>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const drawer = ref(null)
</script>
