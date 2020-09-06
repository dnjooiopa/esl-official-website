<template>
  <div>
    <employee-table />
  </div>
</template>

<script>
import EmployeeTable from './components/EmployeeTable'

export default {
  name: 'Hello World!',
  components: {
    EmployeeTable,
  },
}
</script>

<style>
h1 {
  color: white;
  background-color: black;
}
</style>
