<template>
  <v-card class="mx-auto" max-width="400">
    <v-img :src="PersongeImpor.img" height="200"></v-img>

    <v-card-title> {{ PersongeImpor.name }} </v-card-title>
  </v-card>
</template>

<script>
export default {
  props: ["PersongeImpor"],
};
</script>

<style scoped>
.v-card > *:last-child:not(.v-btn):not(.v-chip):not(.v-avatar) {
  justify-content: center;
  font-family: "Montserrat", sans-serif;
  font-weight: bold;
}
</style>