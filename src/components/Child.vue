<template>
  <div>
    <h1>Child Components</h1>
    <!-- <h2>{{name}}</h2> -->
    <h3 v-for="user in users" :key="user.name">{{user.name}}--{{user.email}}</h3>
  </div>
</template>
<script>
export default {
  name: "Child",
  props: ["users"]
};
</script>