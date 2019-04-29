<template>
  <div>
    首页
    <button @click="btn">获取数据</button>
  </div>
</template>

<script>
export default {
  name: 'home',
  methods: {
    btn () {
      this.$axios.post('/local/app/home.do').then(function (response) {
        console.log(response)
      })
    }
  }
}
</script>

<style scoped>

</style>
