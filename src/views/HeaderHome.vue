<template>
  <div>
    <h2>Home</h2>
    <nav>
      <router-link
        to="/"
        active-class="link--active"
        class="link"
        exact
      >Home</router-link>
      <router-link
        :to="{ name: 'users-id-profile', params: { id: 1 }, query: { lang: 'ja', page: 2}, hash: '#next-user' }"
        active-class="link--active"
        class="link"
        exact
      >Users</router-link>
    </nav>
  </div>
</template>

<style scoped>
.link {
  margin-right: 10px;
}
.link--active {
  font-size: 20px;
}
</style>