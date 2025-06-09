<template>
  <hero />
  <HomeCards />
  <JobListings :limit="3" :show-button="true" />
</template>

<script setup>
import hero from '@/components/hero.vue'
import HomeCards from '@/components/HomeCards.vue'
import JobListings from '@/components/JobListings.vue'
</script>
