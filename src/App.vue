<template>
  <div style="width: 700px; margin: auto; padding-top: 50px;">
    <nav>
      <router-link
        to="/"
        active-class="link--active"
        class="link"
        exact
      >Home</router-link>
      <router-link
        :to="{ name: 'users-profile', params: { id: 1 } }"
        active-class="link--active"
        class="link"
        exact
      >Users</router-link>
    </nav>
    <Home></Home>
    <router-view></router-view>
  </div>
</template>


<style>
.link {
  margin-right: 10px;
}
.link--active {
  font-size: 20px;
}
</style>