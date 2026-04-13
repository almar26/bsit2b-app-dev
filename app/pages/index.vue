<template>
  <div class="d-flex justify-center align-center" style="height: 90vh">
    <v-card class="text-center" width="400" elevation="12">
      <v-icon size="80" color="primary" class="mt-10">mdi-apple</v-icon>

      <v-card-text class="pa-10">
        <v-text-field
          prepend-inner-icon="mdi-account"
          variant="outlined"
          label="Username"
          v-model="username"
        ></v-text-field>

        <v-text-field
          prepend-inner-icon="mdi-account"
          variant="outlined"
          label="Password"
          type="password"
          v-model="password"
        ></v-text-field>

        <v-btn block color="primary" @click="signIn">Sign In</v-btn>
      </v-card-text>
    </v-card>
  </div>
</template>

<script setup>
definePageMeta({
  layout: "auth",
});

const username = ref("");
const password = ref("");

const defaultUsername = ref("admin");
const defaultPassword = ref("admin123");

function signIn() {
  //`alert("Successfully signed in!");`
  //return navigateTo("/prelim");
  if (
    username.value === defaultUsername.value &&
    password.value === defaultPassword.value
  ) {
    navigateTo("/calculate");
  } else {
    alert("Invalid username or password. Please try again.");
  }
}
</script>