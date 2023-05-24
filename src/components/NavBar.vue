<template>
  <v-app-bar app color="#111111" dark flat class="px-8">
    <v-container>
      <v-row justify="center">
        <v-col cols="auto">
          <v-btn text @click="scroll('home')">Home</v-btn>
          <v-btn text @click="scroll('project')">Project</v-btn>
          <v-btn text @click="scroll('about')">about</v-btn>
          <v-btn text @click="scroll('contact')"> contact</v-btn>
        </v-col>
      </v-row>
    </v-container>
   
  </v-app-bar>
</template>

<script>
export default {
  methods: {
    scroll(refName) {
      const element = document.getElementById(refName);
      element.scrollIntoView({ behavior: "smooth" });
    },
  },
};
</script>

<style>
</style>