<template>
  <div class="about">
    <h1>This is an about page</h1>
    <button @click="checkRouteInfo">ルート情報</button>
    <button @click="goToHome">Homeに戻る</button>
  </div>
</template>
<script>
export default {
  name:'AboutName',
  methods:{
    checkRouteInfo(){
      console.log(this.$route)
      console.log(this.$route.path)
      console.log(this.$router)
    },
    goToHome(){
      this.$router.push('/')
    }
  }
}
</script>