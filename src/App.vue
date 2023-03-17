<template>
  <div id="app">
    <instructions />
    <label>
      Input OUTSIDE the component:
      <input type="text" />
    </label>
    <SyncfusionGrid />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import SyncfusionGrid from './components/SyncfusionGrid.vue';
import Instructions from './components/Instructions.vue';

@Component({
  components: {
    SyncfusionGrid,
    Instructions
  },
})
export default class App extends Vue {}
</script>

<style>
@import '~@syncfusion/ej2-base/styles/material.css';
@import '~@syncfusion/ej2-buttons/styles/material.css';
@import '~@syncfusion/ej2-calendars/styles/material.css';
@import '~@syncfusion/ej2-dropdowns/styles/material.css';
@import '~@syncfusion/ej2-inputs/styles/material.css';
@import '~@syncfusion/ej2-navigations/styles/material.css';
@import '~@syncfusion/ej2-popups/styles/material.css';
@import '~@syncfusion/ej2-splitbuttons/styles/material.css';
@import "~@syncfusion/ej2-vue-grids/styles/material.css";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

label {
  display: flex;
  justify-content: center;
  align-items: center;
  background: lightgray;
}

input {
  margin: 20px;
}
</style>
