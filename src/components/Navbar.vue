<template>
  <v-app-bar dark fixed>
    <router-link to="/">
      <v-toolbar-title>
        <v-avatar style="margin-right: .4rem;">
          <v-img src="../assets/logo.png"></v-img>
        </v-avatar>
        Laze
      </v-toolbar-title>
    </router-link>
    <v-spacer/>
    <v-btn text style="border-radius: 0;" class="d-none d-sm-none d-md-flex"><v-icon>mdi-home</v-icon>Home</v-btn>
    <v-spacer/>
    <v-btn large color="blue accent-4" class="login-btn">
      <v-icon>mdi-discord</v-icon>
      Login
    </v-btn>
  </v-app-bar>
</template>
<script>
import { Component, Vue } from 'vue-property-decorator'

@Component({})
export default class Navbar extends Vue {
}
</script>

<style scoped>
.v-icon {
  margin-right: .4rem;
}
.login-btn {
  border-radius: 2rem;
  text-transform: none;
}
</style>
