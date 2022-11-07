<template>
  <div>
    <input type="search" v-model="searchText" @keyup.enter="doSearch" @keyup.delete="doSearch" @keyup.stop="doSearch"/>
    <button @click="doSearch()">조회</button>
    <button type="submit" @click.prevent="doSearch"></button>
  </div>
</template>

<script>
// .stop - event.stopPropagation()
// .prevent - event.preventDefault()
export default {
  components: {},
  data() {
    return {
      searchText: ''
    }
  },
  setup() {},
  created() {},
  mounted() {},
  unmounted () {},
  methods: {
    doSearch() {
      console.log(this.searchText)
    }
  }
}
</script>

<style scoped>

</style>
