<template>
  <div>
    <input type="text" v-bind:value="userId" readonly/>
    <input type="text" :value="userId" readonly/>v-bind 생략 가능
    <br/>
    <img :src="imgSrc" alt="" style="width:100px;height:auto;"/>
    <br />
    <input type="search" v-model="txt1" />
    <button :disabled="txt1 === ''">조회</button>
  </div>
</template>

<script>
export default {
  components: {},
  data () {
    return {
      userId: '012attack',
      imgSrc: 'https://upload.wikimedia.org/wikipedia/commons/f/f1/Vue.png',
      txt1: ''
    }
  },
  setup () {
  },
  created () {
  },
  mounted () {
  },
  unmounted () {
  },
  methods: {}
}
</script>

<style scoped>

</style>
