<template>
  <section class="bg-blue-50 px-4 py-10">
    <div class="container-xl lg:container m-auto">
      <h2 class="text-3xl font-bold text-green-500 mb-6 text-center">Brows Jobs</h2>
      <!-- Show loading spinner while loading is true -->
      <div v-if="state.isLoading" class="text-center text-gray py-6">
        <PulseLoader />
      </div>
      <!-- show jobListing if it's done loading -->
      <div v-else class="grid grid-col-1 md:grid-cols-3 gap-6">
        <jobListing
          v-for="job in state.jobs.slice(0, limit || state.jobs.length)"
          :key="job.id"
          :job="job"
        />
      </div>
    </div>
  </section>
  <section v-if="showButton" class="m-auto max-w-lg my-10 px-6">
    <RouterLink
      to="/jobs"
      class="block bg-black text-white text-center py-4 px-6 rounded-xl hover:bg-gray-700"
      >View All Jobs</RouterLink
    >
  </section>
</template>

<script setup>
import jobListing from './JobListing.vue'
import { reactive, defineProps, onMounted } from 'vue'
import PulseLoader from 'vue-spinner/src/PulseLoader.vue'
import { RouterLink } from 'vue-router'
import axios from 'axios'

defineProps({
  limit: Number,
  showButton: {
    type: Boolean,
    default: false,
  },
})
// const jobs = ref([])
const state = reactive({
  jobs: [],
  isLoading: true,
})

onMounted(async () => {
  try {
    console.log(state.jobs)
    const response = await axios.get('/api/jobs')
    // jobs.value = response.data
    console.log(response)
    state.jobs = response.data
  } catch (error) {
    console.log('error fetching jobs', error)
  } finally {
    state.isLoading = false
  }
})
console.log(state.jobs)
// onMounted(async () => {
//   try {
//     const response = await fetch(`/api/jobs`)
//     // jobs.value = response.data
//     const data = await response.json()
//     state.jobs = data
//   } catch (error) {
//     console.log('error fetching job', error)
//   } finally {
//     state.isLoading = false
//   }
// })
</script>
