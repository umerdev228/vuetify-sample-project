<template>
<!--  <v-app-bar flat>-->
<!--    <v-app-bar-title>-->
<!--      <v-icon icon="mdi-circle-slice-4" />-->

<!--      Base Preset-->
<!--    </v-app-bar-title>-->
<!--  </v-app-bar>-->

  <v-app>
    <v-app-bar app>
      Title
    </v-app-bar>

    <v-navigation-drawer
      color="#09151E"
      permanent
      expand-on-hover
      app
    >
      <v-divider></v-divider>
      <v-list nav dense>
        <v-list-item link href="#">
          hello world
        </v-list-item>
        <v-list-item link href="#">
          <v-list-item-title class="title">Blue</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <default-view />

  </v-app>

</template>

<script setup>
import DefaultView from './View.vue'

  //
</script>
