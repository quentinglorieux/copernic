<template>
  <div>
    <div v-for="item in items" v-bind:key="item.id">
      <MemberItem :memberData="item"> </MemberItem>
    </div>
  </div>
</template>

<script>
import json from "~/assets/json/member.json";

export default {
  name: "MemberPage",
  data() {
    return {
      items: json,
    };
  },
};
</script>
