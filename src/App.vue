<template>
  <div id="app">
    <div class="container">
      <roll-button></roll-button>
      <show-dice></show-dice>
      <table-view></table-view>
      <reset-button></reset-button>
    </div>
    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>-->
  </div>
</template>

<script>
import RollButton from "./components/RollButton.vue";
import ShowDice from "./components/ShowDice.vue";
import TableView from "./components/TableView.vue";
import ResetButton from "./components/ResetButton.vue";

export default {
  props: ["dice"],
  name: "app",
  components: {
    RollButton,
    ShowDice,
    TableView,
    ResetButton
  }
};
</script>

<style>
</style>
