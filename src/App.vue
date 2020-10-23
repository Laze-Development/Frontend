<template>
  <v-app>
    <Navbar/>
  </v-app>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator"
import Navbar from "./components/Navbar.vue";

@Component({
  components: {
    Navbar
  }
})
export default class App extends Vue {
}
</script>
<style>
.router-link-active {
  color: white !important;
  text-decoration: none !important;
}
</style>
