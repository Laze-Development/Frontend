<template>
  <v-navigation-drawer v-model="$store.state.sidebarDrawer" dark color="grey darken-4">
    <v-list>
      <v-list-item class="px-2">
        <v-list-item-avatar>
          <v-img src="../assets/logo.png"></v-img>
        </v-list-item-avatar>
        <v-list-item-title class="title">Laze</v-list-item-title>
        <v-btn text @click="$store.state.sidebarDrawer = false;">
          <v-icon>mdi-chevron-right</v-icon>
        </v-btn>
      </v-list-item>
    </v-list>
    <template v-slot:append>
      <div>
        <v-btn block color="blue accent-3">
          Login
        </v-btn>
      </div>
    </template>
  </v-navigation-drawer>
</template>
<script lang="ts">
import { Vue, Component } from "vue-property-decorator";

@Component({
  data: () => ({
    drawer: true
  })
})
export default class Sidebar extends Vue {
}
</script>
