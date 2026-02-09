<template>
  <div>
    <h1>Welcome to My Nuxt App</h1>
    <v-row>
      <v-col cols="12" md="3">
        <v-card height="120" color="blue">
          <v-card-text>
            <v-row>
              <v-col cols="6">
                <v-icon size="90">mdi-account-circle</v-icon>
              </v-col>
              <v-col cols="6">
                <v-row no-gutters>
                  <v-col cols="12" class="text-h6 text-right"> STUDENT </v-col>
                  <v-col cols="12" class="text-h3 text-right font-weight-bold">
                    250
                  </v-col>
                </v-row>
              </v-col>
            </v-row>
          </v-card-text>
        </v-card>
      </v-col>
      <v-col cols="12" md="3">
        <v-card height="120" color="red">
          <v-card-text>
            <v-row>
              <v-col cols="6">
                <!-- ICON -->
                <v-sheet color="white" height="90"> </v-sheet>
              </v-col>
              <v-col cols="6">
                <v-row dense>
                  <v-col cols="12">
                    <!-- LABEL -->
                    <v-sheet color="white" height="40"> </v-sheet>
                  </v-col>
                  <v-col cols="12">
                    <!-- VALUE/AMOUNT -->
                    <v-sheet color="white" height="40"> </v-sheet>
                  </v-col>
                </v-row>
              </v-col>
            </v-row>
          </v-card-text>
        </v-card>
      </v-col>
      <v-col cols="12" md="3">
        <v-card height="120" color="green"> </v-card>
      </v-col>
      <v-col cols="12" md="3">
        <v-card height="120" color="purple"></v-card>
      </v-col>
    </v-row>
  </div>
</template>

<script setup>
const headers = [
  { title: "Pyramid", value: "name" },
  { title: "Location", value: "location" },
  { title: "Construction Date", value: "constructionDate" },
  {
    title: "Dimensions",
    align: "center",
    children: [
      { title: "Height(m)", value: "height" },
      { title: "Base(m)", value: "base" },
      { title: "Volume(m³)", value: "volume" },
    ],
  },
];

const items = [
  {
    name: "Great Pyramid of Giza",
    location: "Egypt",
    height: "146.6",
    base: "230.4",
    volume: "2583285",
    constructionDate: "c. 2580–2560 BC",
  },
  {
    name: "Pyramid of Khafre",
    location: "Egypt",
    height: "136.4",
    base: "215.3",
    volume: "1477485",
    constructionDate: "c. 2570 BC",
  },
  {
    name: "Red Pyramid",
    location: "Egypt",
    height: "104",
    base: "220",
    volume: "1602895",
    constructionDate: "c. 2590 BC",
  },
  {
    name: "Bent Pyramid",
    location: "Egypt",
    height: "101.1",
    base: "188.6",
    volume: "1200690",
    constructionDate: "c. 2600 BC",
  },
  {
    name: "Pyramid of the Sun",
    location: "Mexico",
    height: "65",
    base: "225",
    volume: "1237097",
    constructionDate: "c. 200 CE",
  },
];
</script>

<style>
</style>