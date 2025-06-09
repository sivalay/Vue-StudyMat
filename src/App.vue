<template>
  <Navbar />
  <RouterView />
</template>

<script setup>
import Navbar from './components/Navbar.vue'
import { RouterView } from 'vue-router'
</script>

<!-- study-material
<template>
  <v-btn :active-color="'red'"> Button </v-btn>
  <v-text-field :bg-color="'red'" />
  <span class="text-2xl">Hello</span>
  <v-text-field :bg-color="red"></v-text-field>
</template> -->
