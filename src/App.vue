<template>
  <v-app id="inspire">
    <v-navigation-drawer
      v-model="drawer"
      fixed
      app
    >
      <v-list dense>
        <router-link
          :to="{name:'Home'}"
          class="side_bar_link"
        >
          <v-list-tile>
            <v-list-tile-action>
              <v-icon>home</v-icon>
            </v-list-tile-action>
            <v-list-tile-content>Home</v-list-tile-content>
          </v-list-tile>
        </router-link>
        <router-link
          :to="{name: 'Contact'}"
          class="side_bar_link"
        >
          <v-list-tile>
            <v-list-tile-action>
              <v-icon>contact_mail</v-icon>
            </v-list-tile-action>
            <v-list-tile-content>Contact</v-list-tile-content>
          </v-list-tile>
        </router-link>
      </v-list>
    </v-navigation-drawer>
    <v-toolbar
      color="indigo"
      dark
      fixed
      app
    >
    </v-toolbar>
  </v-app>
</template>

<script>
import '@/assets/stylesheets/main.scss'

export default {
  data: () => ({
    drawer: null
  }),
  props: {
    source: String
  }
}
</script>
