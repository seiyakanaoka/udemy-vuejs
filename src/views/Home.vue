<template>
  <div>
    <h3>Home</h3>
    <h3>Hello</h3>
    <button @click="toUsers">Usersのページにいく</button>
  </div>
</template>

<script>
export default {
  methods: {
    toUsers() {
      this.$router.push({
        name: 'users-id-profile',
        params: { id: 1 }
      });
    }
  }
}
</script>