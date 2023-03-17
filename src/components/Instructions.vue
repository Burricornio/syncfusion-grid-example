<template>
  <div>
    <h1>Instructions</h1>
    <ul>
      <li>
        Filter any of the columns entering a value.
      </li>
      <li>
        All input fields in the application lose the focus property.
      </li>
    </ul>
    <hr>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component
export default class Instructions extends Vue {}
</script>

<style scoped>

  div {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  h1 {
    margin: 25px 0 0 0;
    text-transform: uppercase;
    background: green;
    color: white;
    padding: 10px;
  }

  ul {
    width: 450px;
    background-color: lightgoldenrodyellow;
    padding: 20px;
    text-align: left;
  }

  li {
    padding: 5px;
  }

</style>
