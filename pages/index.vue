<template>
  <div>
    <v-container class="grey lighten-5">
      <v-row>
        <v-col
          sm="12"
          md="4"
          lg="4"
          v-for="(personge, index) in Personges"
          :key="index"
        >
          <Cards :PersongeImpor="personge"></Cards>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
import Cards from "../components/Cards.vue";
import Personge from "../personges"

export default {
  name: "IndexPage",
  data() {
    return {
      Personges: Personge
    };
  }
};
component: {
  Cards;
}
</script>
