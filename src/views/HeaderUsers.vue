<template>
  <nav>
    <h2>Usersのヘッダー</h2>
    <router-link to="/" active-class="link--active" class="link" exact>Home</router-link>
    <router-link to="/users" active-class="link--active" class="link" exact>Users</router-link>
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