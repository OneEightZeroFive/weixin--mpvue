<template>
    <div>
        <input v-model="name" />
        <p>{{name}}</p>
        <button @click="sendName">传递数据</button>
    </div>
</template>

<script>
import store from "../utils/store";
export default {
  data() {
    return {
      name: "ly"
    };
  },
  methods: {
    sendName() {
      var name = this.name;
      store.commit("sendName", name);
    }
  }
};
</script>

<style>
</style>
