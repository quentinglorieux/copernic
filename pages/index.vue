<template>
  <div class="font-bold text-xl mb-2 mt-40 text-center">
  <NuxtLink class="button-menu" to="/join-us"> Jobs </NuxtLink>
  <NuxtLink class="button-menu" to="/publications"> Publications </NuxtLink>
  <NuxtLink class="button-menu" to="/research"> Research </NuxtLink>
  <NuxtLink class="button-menu" to="/team"> Team </NuxtLink>
  </div>
</template>


<script>
export default{
  name: "IndexPage"
  }
</script> 

<style lang="postcss" scoped>
.button-menu {
  @apply inline-block bg-gray-300 rounded-full px-3 py-1 text-sm font-semibold text-gray-800;
  &:hover {
    @apply bg-gray-50 text-black;
  }
}

</style>