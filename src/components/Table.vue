<template>
  <div>
    <h1>--- Tables ---</h1>
  </div>
  <input v-model="search" type="number" id="Input" placeholder="Search table" />
  <div>
    <ul v-if="search">
      <li v-for="index in 10">
        {{ search }}*{{ index }} = {{ search * index }}
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  name: 'Table',
  data() {
    return {
      search: '',
    }
  },
}
</script>
<style scoped>
li {
  list-style-type: none;
}
</style>
