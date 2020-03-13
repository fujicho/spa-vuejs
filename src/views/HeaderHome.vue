<template>
  <nav>
    <h2>Homeのヘッダー</h2>
    <router-link to="/" active-class="link--active" class="link" exact>Home</router-link>
    <router-link :to="{name: 'users-id-profile',params: {id:1},hash:'#next-user'}"
    active-class="link--active" class="link" exact>users</router-link>
    <button @click="increment">+1</button>
    <button @click="decrement">-1</button>
  </nav>
</template>

<script>
export default {
  methods: {
    increment(){
      this.$store.state.count++
    },
    decrement(){
      this.$store.state.count--
    },
  }
}
</script>

<style scoped> 
.link {
  margin-right: 10px;
}
.link--active{
  font-size: 20px;
}
</style>