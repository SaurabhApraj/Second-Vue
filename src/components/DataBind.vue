<template>
  <div>
    <!-- <h1>{{message}}</h1> -->
    <!-- <input type="text" v-model="message" placeholder="Message" /> -->
    <p style="white-space:pre-line">{{message}}</p>
    <textarea type="text" v-model="message"></textarea>
  </div>
</template>
<script>
export default {
  name: "DataBind",
  data() {
    return {
      message: ""
    };
  }
};
</script>