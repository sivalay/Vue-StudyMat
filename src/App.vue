<script setup>
import Navbar from './components/Navbar.vue'
import hero from './components/hero.vue'
import HomeCards from './components/HomeCards.vue'
import JobListings from './components/JobListings.vue'
</script>

<template>
  <!-- <v-btn :active-color="'red'"> Button </v-btn>
  <v-text-field :bg-color="'red'" />
  <span class="text-2xl">Hello</span> -->
  <!-- <v-text-field :bg-color="red"></v-text-field> -->
  <Navbar />
  <hero />
  <HomeCards />
  <JobListings :limit="3" :show-button="true" />
</template>
