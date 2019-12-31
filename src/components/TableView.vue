<template>
  <div class="columns is-centered" v-show="dice.length">
    <div class="column is-narrow">
      <table class="table is-bordered">
        <thead>
          <!-- <tr>
            <td>Section 1</td>
          </tr>-->
        </thead>
        <tbody>
          <tr>
            <th>One</th>
            <td></td>
          </tr>
          <tr>
            <th>Two</th>
            <td></td>
          </tr>
          <tr>
            <th>Three</th>
            <td></td>
          </tr>
          <tr>
            <th>Four</th>
            <td></td>
          </tr>
          <tr>
            <th>Five</th>
            <td></td>
          </tr>
          <tr>
            <th>Six</th>
            <td></td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<script>
export default {
  name: "TableView",
  props: ["dice"]
};
</script>

<style>
</style>