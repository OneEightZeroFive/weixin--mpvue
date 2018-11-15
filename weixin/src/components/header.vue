<template>
    <header>{{name}}</header>
</template>

<script>
import store from "../utils/store";

export default {
  computed: {
    name() {
      return store.state.name;
    }
  }
};
</script>

<style>
header {
  line-height: 50px;
  height: 50px;
  width: 100%;
  text-align: center;
  color: white;
  background-color: red;
}
</style>
