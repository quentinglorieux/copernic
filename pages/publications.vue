<template>
  <div>
    <div v-for="item in items" v-bind:key="item.id">
      <PublicationItem v-bind:publication="item"> </PublicationItem>
    </div>
  </div>
</template>


<script>
import json from "~/assets/json/publication.json";

export default {
  name: "PubliPage",
  data() {
    return {
      items: json,
    };
  },
};
</script>



<style lang="postcss" scoped>
.container {
  padding: 20px;
  width: 100%;
  margin: 0 auto;
}
.button-filter {
  @apply bg-transparent focus:text-emerald-400  text-gray-200 hover:text-gray-400 py-2 px-4 text-base; /* since v3 */
}
</style>

