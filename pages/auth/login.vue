<template>
  <form @submit.prevent="login">
    <label for="username">Username:</label>
    <input v-model="username" type="text" id="username" />

    <label for="password">Password:</label>
    <input v-model="password" type="password" id="password" />

    <button type="submit">Login</button>
  </form>
</template>

<script>
export default {
  data() {
    return {
      username: '',
      password: '',
    };
  },
  methods: {
    login() {
      // Implement your login logic here
    },
  },
};
</script>
