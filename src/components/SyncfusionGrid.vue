<template>
  <div>

    <label>
      Input INSIDE the component:
      <input type="text" />
    </label>

    <ejs-grid ref='grid' :dataSource="people" :allowFiltering='true' :filterSettings='filterSettings'>
        <e-columns>
          <e-column field='name' headerText='Name' width='150'></e-column>
          <e-column field='surname' headerText='Surname' width='120'></e-column>
        </e-columns>
    </ejs-grid>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import { GridPlugin, Filter } from "@syncfusion/ej2-vue-grids";

Vue.use(GridPlugin);

@Component({
  provide: {
      grid: [Filter ]
  }
})
export default class SyncfusionGrid extends Vue {

  filterSettings = { type: 'Menu' }

  people = [
    {
      name: "Mike",
      surname: "Gonzalez"
    },
    {
      name: "Ellie",
      surname: "Joel"
    },
    {
      name: "John",
      surname: "Doe"
    },
  ]
}
</script>
