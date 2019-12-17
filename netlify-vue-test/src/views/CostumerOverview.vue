<template>
  <div class="table">
    <h1>Table template</h1>
    <TableStructure></TableStructure>
  </div>
</template>

<script>
// @ is an alias to /src
import TableStructure from "@/components/Table.vue";

export default {
  name: "table",
  components: {
    TableStructure
  }
};
</script>
