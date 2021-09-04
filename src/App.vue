<template>
  <div>
    <PersonelTable />
  </div>
</template>

<script>
import PersonelTable from "./components/PersonelTable.vue";

export default {
  name: "App",
  components: { PersonelTable },
};
</script>

<style>
body {
  background-color: whitesmoke;
}
</style>
