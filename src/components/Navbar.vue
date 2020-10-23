<template>
  <v-app-bar dark fixed>
    <router-link to="/">
    <v-toolbar-title>
      <v-avatar><v-img src="../assets/logo.png"></v-img></v-avatar>
      Laze
    </v-toolbar-title>
    </router-link>
  </v-app-bar>
</template>
<script>
import { Component, Vue } from 'vue-property-decorator'

@Component({})
export default class Navbar extends Vue {}
</script>
