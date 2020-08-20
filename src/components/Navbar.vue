<template>
  <nav>
    <v-app-bar bg-color="white" app>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      <v-toolbar-title class="text-uppercase ">
        <v-avatar size="30">
          <img src="../assets/fcmb-logo.png" alt="" />
        </v-avatar>
        <span class="font-weight-light pl-4">FCMB: Mobile Banking</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <!-- <v-text-field
        flat
        hide-details
        append-icon="mdi-magnify"
        placeholder="Search"
        outlined
        dense
        @click:append="search"
        class="hidden-sm-and-down border-radius"
      ></v-text-field> -->
      <v-spacer></v-spacer>
      <v-tooltip bottom>
        <template v-slot:activator="{ on }">
          <v-btn icon v-on="on" class="mr-7">
            <v-icon size="25">mdi-bell</v-icon></v-btn
          >
        </template>
        <span>Notifications</span>
      </v-tooltip>

      <!-- <v-avatar> -->
      <img src="../assets/owner.png" alt="" />
      <!-- </v-avatar> -->
      <!-- <v-avatar> -->
      <img src="../assets/Vector.png" class="icon-image" alt="" />
      <!-- </v-avatar> -->

      <v-menu offset-y>
        <template v-slot:activator="{ on }">
          <v-btn text v-on="on">
            <img src="../assets/Rectangle 4.png" class="icon-image" alt="" />
            <span>Menu</span>
            <v-icon left>expand_more</v-icon>
          </v-btn>
        </template>
        <v-list flat>
          <v-list-item
            v-for="link in links"
            :key="link.text"
            router
            :to="link.route"
            active-class="border"
          >
            <v-list-item-title>{{ link.text }}</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
      <v-btn text>
        <span>Exit</span>
        <v-icon right>exit_to_app</v-icon>
      </v-btn>
    </v-app-bar>
    <v-navigation-drawer
      v-model="drawer"
      dark
      app
      class=" darken-4"
      width="100"
    >
      <v-layout column align-center>
        <v-flex class="mt-5">
          <v-avatar size="30">
            <img src="../assets/bank-logo.png" alt="" />
          </v-avatar>
          <!-- <p class="white--text subheading mt-1 text-center">Username</p> -->
        </v-flex>
        <v-flex class="mt-4 mb-4">
          <!-- <Popup /> -->
        </v-flex>
      </v-layout>
      <v-list flat>
        <v-list-item
          v-for="link in links"
          :key="link.text"
          router
          :to="link.route"
          active-class="border"
        >
          <v-list-item-action>
            <v-icon class="mx-auto">{{ link.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>{{ link.text }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
      <v-divider></v-divider>
      <v-list flat>
        <v-list-item
          v-for="link in links"
          :key="link.text"
          router
          :to="link.route"
          active-class="border"
        >
          <v-list-item-action>
            <v-icon>{{ link.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>{{ link.text }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
  </nav>
</template>
<script>
// import Popup from './Popup.vue'
export default {
  data: () => ({
    drawer: true,
    links: [
      { icon: "dashboard", route: "/" },
      { icon: "folder", route: "/projects" },
      { icon: "person", route: "/team" },
    ],
  }),
  //   components: {
  //   Popup
  // },
};
</script>
<style scoped>
.border {
  border-left: 4px solid #0ba518;
}
.nav-drawer {
  background: #052231;
}
.icon-image {
  padding-left: 90px;
}
@media (max-width: 768px) {
  .icon-img {
    visibility: hidden;
  }
}
</style>
