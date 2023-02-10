<template>
  <v-app>
    <v-app-bar app>
      <v-toolbar-title>Events</v-toolbar-title>

      <v-text-field placeholder="Zoek evenement" class="ml-8" style="max-width: 350px" prepend-inner-icon="mdi-magnify"
        outlined rounded dense hide-details />

      <v-spacer></v-spacer>
      <v-btn>Create event</v-btn>
    </v-app-bar>
    <v-main>
      <slot />
    </v-main>
  </v-app>
</template>

<static-query>
query {
  metadata {
    siteName,
    siteDescription
  }
}
</static-query>

<style>

</style>
