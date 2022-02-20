<template>
  <div>
    <div v-for="item in items" v-bind:key="item.id">
      <JobItem v-bind:jobData="item" > </JobItem>  
    </div>
  </div>
</template>

<script>
import json from "~/assets/json/job.json";

export default {
  name: "JobPage",
  data() {
    return {
      items: json,
    };
  },
};
</script>


