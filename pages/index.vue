<template>
  <div style="margin: 100px;">
    <div v-if="$auth.loggedIn">
      {{ $auth.user.email }}
      <v-btn @click="$auth.logout()">Logout</v-btn>
    </div>
    <div v-else>
      <v-btn @click="login">Login</v-btn>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
export default Vue.extend({
  methods: {
    login() {
      this.$auth.loginWith("google");
    }
  }
});
</script>
