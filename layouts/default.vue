<template>
  <div>
    <HeroBar />
    <Nuxt />
    <div class="button-menu-layout">
      <NuxtLink to="/"> Home </NuxtLink>
    </div>
  </div>
</template>

<script>
export default {
  head: {
    title: "Test Lab",
    meta: [
      {
        hid: "description",
        name: "description",
        content: "Content",
      },
    ],
  },
};
</script>

<style lang="postcss" scoped>
.button-menu-layout {
  @apply mt-10 inline-block self-center bg-gray-300 px-3 py-1 text-sm font-semibold text-gray-800;
  &:hover {
    @apply bg-gray-50 text-black;
  }
}
</style>