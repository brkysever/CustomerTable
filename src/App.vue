<template>
  <div>
    <CustomerTable />
  </div>
</template>

<script>
import CustomerTable from "./components/CustomerTable.vue";

export default {
  name: "App",
  components: { CustomerTable },
};
</script>

<style>
body {
  background-color: #f1f2f7;
}
</style>
