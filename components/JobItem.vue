<template>
  <div class="p-4">
    <div class="max-w-5xl rounded overflow-hidden shadow-lg mb-4 bg-gray-500">
      <div class="px-6 py-4 pb-2">
        <div class="font-bold text-xl mb-2 text-center">
          {{ jobData.title }}
        </div>
        <p class="text-gray-300 text-base" v-html="jobData.description"></p>
      </div>

      <div class="px-6 py-4">
        <span class="badge mr-2">{{ jobData.type }}</span>
        <span class="badge mr-2"> {{ jobData.location }}</span>
        <span class="badge"> {{ jobData.duration }} months </span>
      </div>
    </div>
  </div>
</template>

<style lang="postcss" scoped>
.badge {
  @apply inline-block bg-gray-300 rounded-full px-3 py-1 text-sm font-semibold text-gray-800;
  &:hover {
    @apply bg-gray-50;
  }
}
</style>

<script>
export default {
  name: "JobItem",
  props: {
    jobData: '',
  },
};
</script>
