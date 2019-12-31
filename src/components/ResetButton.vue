<template>
  <div class="hero">
    <div class="hero-body has-text-centered">
      <button class="button is-danger is-outlined is-small" :disabled="!!diceData.length">Reset</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "ResetButton",
  props: {
    diceData: {
      type: Array,
      required: true
    }
  }
  //   watch: {
  //     diceData: {
  //       handler(newValue, oldValue) {
  //         // eslint-disable-next-line
  //         console.log(newValue.length);
  //       },
  //       immediate: true
  //     }
  //   }
};
</script>

<style>
</style> 