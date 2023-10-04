<template>
  <div v-if="!$store.state.isAuthenticated">
    <login />
  </div>
  <div v-else>
    <p>Welcome, you are logged in!</p>
    <button @click="logout">Logout</button>
  </div>
</template>

<script>
import login from './auth/login.vue';

export default {
  components: {
    login,
  },
  methods: {
    logout() {
      this.$store.commit('logout');
    },
  },
};
</script>
