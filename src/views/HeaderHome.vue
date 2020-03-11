<template>
  <nav>
    <h2>Homeのヘッダー</h2>
    <router-link to="/" active-class="link--active" class="link" exact>Home</router-link>
    <router-link :to="{name: 'users-id-profile',params: {id:1},hash:'#next-user'}"
    active-class="link--active" class="link" exact>users</router-link>
  </nav>
</template>

<style scoped> 
.link {
  margin-right: 10px;
}
.link--active{
  font-size: 20px;
}
</style>