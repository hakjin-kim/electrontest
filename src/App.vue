<template>
  <div id="app">
    <!--<div id="toolbar">-->
    <v-navigation-drawer
            v-model="drawerRight"
            fixed
            right
            clipped
            app
    >
      <v-list dense>
        <!--<router-link to="/" tag="v-list-tile">-->
        <v-list-tile to="/" @click.stop="right = !right" >
          <v-list-tile-action>
            <v-icon>exit_to_app</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title>Temporary Drawer</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
        <!--</router-link>-->

        <!--<router-link to="/about" tag="v-list-tile">-->
        <v-list-tile to="/about" @click.stop="right = !right">
          <v-list-tile-action>
            <v-icon>backspace</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title>Others</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
        <!--</router-link>-->
      </v-list>
    </v-navigation-drawer>
      <v-toolbar
              color="blue-grey"
              dark
              fixed
              app
              clipped-right
      >
        <!--<v-toolbar-side-icon @click.stop="drawer = !drawer"></v-toolbar-side-icon>-->
        <v-toolbar-title>Toolbar</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-toolbar-side-icon @click.stop="drawerRight = !drawerRight"></v-toolbar-side-icon>
      </v-toolbar>


    <!--</div>-->
    <!--<div id="nav">
      <router-view/>
    </div>-->
    <main>
      <v-content>
      <router-view></router-view>
      </v-content>
    </main>

  </div>
</template>



<!--<template>
  <v-app id="inspire">

    <v-content>
      <v-container fluid fill-height>
        <v-layout justify-center align-center>
          <v-flex shrink>
            <v-tooltip right>
              <template v-slot:activator="{ on }">
                <v-btn :href="source" icon large target="_blank" v-on="on">
                  <v-icon large>code</v-icon>
                </v-btn>
              </template>
              <span>Source</span>
            </v-tooltip>
            <v-tooltip right>
              <template v-slot:activator="{ on }">
                <v-btn icon large href="https://codepen.io/johnjleider/pen/KQrPKJ" target="_blank" v-on="on">
                  <v-icon large>mdi-codepen</v-icon>
                </v-btn>
              </template>
              <span>Codepen</span>
            </v-tooltip>
          </v-flex>
        </v-layout>
      </v-container>
    </v-content>
    <v-navigation-drawer
            v-model="right"
            right
            temporary
            fixed
    ></v-navigation-drawer>
    <v-footer color="blue-grey" class="white&#45;&#45;text" app>
      <span>Vuetify</span>
      <v-spacer></v-spacer>
      <span>&copy; 2017</span>
    </v-footer>
  </v-app>
</template>-->

<script>
  export default {
    data: () => ({
      drawer: null,
      drawerRight: null,
      right: false,
      left: false
    }),
    props: {
      source: String
    }
  }
</script>