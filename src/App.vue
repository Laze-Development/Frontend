<template>
  <v-app>
    <Sidebar class="d-inline d-sm-inline d-md-none"/>
    <Navbar class="d-none d-sm-none d-md-inline"/>
    <v-btn v-if="!$store.state.sidebarDrawer" fab bottom left large dark class="d-flex d-sm-flex d-md-none drawer-btn"
           fixed
           @click="$store.state.sidebarDrawer = true">
      <v-icon>mdi-arrow-right-thick</v-icon>
    </v-btn>
    <v-btn fab bottom right large dark class="d-flex d-sm-flex d-md-none" fixed>
      <v-icon>mdi-home</v-icon>
    </v-btn>
  </v-app>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator"
import Navbar from "./components/Navbar.vue";
import Sidebar from "./components/Sidebar.vue";

@Component({
  components: {
    Navbar,
    Sidebar
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
