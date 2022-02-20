<template>
  <div>
    <div v-for="item in items" v-bind:key="item.id">
      <ResearchItem :researchData="item"> </ResearchItem>
    </div>
  </div>
</template>

<script>
import json from "~/assets/json/research.json";

export default {
  name: "ResearchPage",
  data() {
    return {
      items: json,
    };
  },
};
</script>
