<template>
  <div>
    <h1>Calculate Page</h1>
    <v-card>
      <v-card-text>
        <v-text-field
          label="Enter 1st number"
          v-model="firstNumber"
        ></v-text-field>

        <v-text-field
          label="Enter 2nd number"
          v-model="secondNumber"
        ></v-text-field>

        <v-text-field label="Total" disabled v-model="total"></v-text-field>

        <v-btn @click="calculateTotal">Calculate</v-btn>
      </v-card-text>
    </v-card>
  </div>
</template>

<script setup>
const firstNumber = ref(0);
const secondNumber = ref(0);
const total = ref(0);

// Function to calculate the total
function calculateTotal() {
  total.value = Number(firstNumber.value) + Number(secondNumber.value);
}
</script>

<style>
</style>