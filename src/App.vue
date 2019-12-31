<template>
  <div id="app">
    <div class="container">
      <roll-button @diceData="triggerMyCustomEvent"></roll-button>
      <show-dice v-show="diceArray.length"></show-dice>
      <table-view v-show="diceArray.length" :diceData="diceArray"></table-view>
      <reset-button :diceData="diceArray"></reset-button>
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
  name: "app",
  components: {
    RollButton,
    ShowDice,
    TableView,
    ResetButton
  },
  data() {
    return {
      diceArray: []
    };
  },
  methods: {
    // updateMessage(variable) {
    //   this.childData = variable;
    // }
    triggerMyCustomEvent(data) {
      this.diceArray = data;
    }
  }
};
</script>

<style>
</style>
