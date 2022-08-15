<template>
  <v-app id="inspire">
    <v-navigation-drawer
      v-model="drawer"
      app
    >
      <!--  -->
    </v-navigation-drawer>

    <v-app-bar app>
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>

      <v-toolbar-title>Application</v-toolbar-title>
    </v-app-bar>

    <v-main>
      <!--  -->
    <Card></Card>
    </v-main>
  </v-app>
</template>

<script>
import Card from "./components/CardComponent.vue"
  export default {
    components:{
      Card,
    },
    data: () => ({ drawer: null }),
  }
</script>