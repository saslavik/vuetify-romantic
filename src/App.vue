<template>
  <v-app id="inspire">
    <v-container>
      <v-app-bar
        color="blue"
        app
        shrink-on-scroll
        prominent
        src="https://picsum.photos/1920/1080?random"
        fade-img-on-scroll
        dark
      >
        <template v-slot:img="{ props }">
          <v-img
            v-bind="props"
            gradient="to top right, rgba(74, 56, 235,.7), rgba(74, 56, 235,.7)"
          ></v-img>
        </template>
        <v-app-bar-nav-icon></v-app-bar-nav-icon>

        <v-toolbar-title>ROMANTIC TUR</v-toolbar-title>

        <v-spacer></v-spacer>

        <v-tabs
          v-model="tab"
          right
          height='58px'
          bottom
        >
          <v-tab
            v-for="link in links"
            :key="link"
          >
            {{ link }}
          </v-tab>
        </v-tabs>
      </v-app-bar>

      <v-main>
        <br>test<br><br><br><br><br><br><br>test<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
      </v-main>
    </v-container>
  </v-app>
</template>

<script>
  export default {
    data: () => ({
      links: [
        'Dashboard',
        'Messages',
        'Profile',
        'Updates',
      ],
    }),
  }
</script>
