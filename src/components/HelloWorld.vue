<template>
  <v-container>
    <v-layout
      text-xs-center
      wrap
    >
      <!--<v-flex xs12>
        <v-img
          :src="require('../assets/logo.svg')"
          class="my-3"
          contain
          height="200"
        ></v-img>
      </v-flex>-->


      <v-flex mb-4>
        <h1 class="display-2 font-weight-bold mb-3">
          Welcome to Vuetify
        </h1>
        <p class="subheading font-weight-regular">
          For help and collaboration with other Vuetify developers,
          <br>please join our online
          <a href="https://community.vuetifyjs.com" target="_blank">Discord Community</a>
        </p>
      </v-flex>

        <!-- <v-flex
          mb-5
          xs12
        >
         <h2 class="headline font-weight-bold mb-3">What's next?</h2>

          <v-layout justify-center>
              <router-link v-for="(next, i) in whatsNext"
                           :key="i"
                           :to="'https://vuetifyjs.com' + next.href"
              >{{ next.text }} <v-tab></v-tab></router-link>
            &lt;!&ndash;<a
              v-for="(next, i) in whatsNext"
              :key="i"
              :href="next.href"
              class="subheading mx-3"
              target="_self"
            >
              {{ next.text }}
            </a>&ndash;&gt;
          </v-layout>
        </v-flex>

        <v-flex
          xs12
          mb-5
        >
          <h2 class="headline font-weight-bold mb-3">Important Links</h2>

          <v-layout justify-center>
            <a
              v-for="(link, i) in importantLinks"
              :key="i"
              :href="link.href"
              class="subheading mx-3"
              target="_blank"
            >
              {{ link.text }}
            </a>
          </v-layout>
        </v-flex>

        <v-flex
          xs12
          mb-5
        >
          <h2 class="headline font-weight-bold mb-3">Ecosystem</h2>

          <v-layout justify-center>
            <a
              v-for="(eco, i) in ecosystem"
              :key="i"
              :href="eco.href"
              class="subheading mx-3"
              target="_blank"
            >
              {{ eco.text }}
            </a>
          </v-layout>
        </v-flex>-->
      </v-layout>

        <!--<router-view></router-view>-->
  </v-container>
</template>
<!--<script src="https://unpkg.com/vue-router@3.0.1/dist/vue-router.js"></script>-->
<script>

  export default {
    data: () => ({
      ecosystem: [
        {
          text: 'vuetify-loader',
          href: 'https://github.com/vuetifyjs/vuetify-loader'
        },
        {
          text: 'github',
          href: 'https://github.com/vuetifyjs/vuetify'
        },
        {
          text: 'awesome-vuetify',
          href: 'https://github.com/vuetifyjs/awesome-vuetify'
        }
      ],
      importantLinks: [
        {
          text: 'Documentation',
          href: 'https://vuetifyjs.com'
        },
        {
          text: 'Chat',
          href: 'https://community.vuetifyjs.com'
        },
        {
          text: 'Made with Vuetify',
          href: 'https://madewithvuetifyjs.com'
        },
        {
          text: 'Twitter',
          href: 'https://twitter.com/vuetifyjs'
        },
        {
          text: 'Articles',
          href: 'https://medium.com/vuetify'
        }
      ],
      whatsNext: [
        {
          text: 'Explore components',
          href: '/components/api-explorer'
        },
        {
          text: 'Select a layout',
          href: '/layout/pre-defined'
        },
        {
          text: 'Frequently Asked Questions',
          href: '/getting-started/frequently-asked-questions'
        }

      ]
    })
  }

/*

  var routes = [

    { path: '/main', component: { template: '<div>main</div>' } },
    { path: '/login', component: { template: '<div>login</div>' } }
  ];

  var router = new VueRouter({
    routes
  });
  // 뷰 라우터를 인스턴스에 등록
  var test = new Vue({
    router
  }).$mount('#test');
*/

</script>

<style>

</style>
