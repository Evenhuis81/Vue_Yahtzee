<template>
  <div class="hero">
    <div class="hero-body has-text-centered">
      <h1 class="title">Yahtzee</h1>
      <button class="button is-danger is-rounded" @click="rolledDice">{{ buttonMsg }}</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      buttonMsg: "Roll the dice!",
      dice: []
    };
  },
  methods: {
    rolledDice() {
      this.dice = [];
      this.buttonMsg = "Roll again!";
      for (let index = 1; index < 6; index++) {
        const dicevalue = Math.ceil(Math.random() * 6);
        this.dice.push(dicevalue);
      }
    }
  }
};
</script>

<style>
</style>