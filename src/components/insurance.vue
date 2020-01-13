<template>
  <v-container fluid>

    <v-row
      class="lg-6"
      no-gutters
    >
      <v-col
        :key="1"
        :cols="2"
      >
        <v-card
          class="pa-2"
          outlined
          tile
        >
          <v-flex xs12>
            <v-img
              :src="require('../assets/mypic.jpg')"
              class="my-3"
              contain
              height="200"
            ></v-img>
          </v-flex>
        </v-card>
      </v-col>
      <v-col
        :key="2"
        :cols="8"
      >
        <v-layout
          text-center
          wrap
        >
          <v-flex mb-4>
            <h1 class="display-2 font-weight-bold mb-3">
              Compare Insurance
            </h1>
            <p class="subheading font-weight-regular">
              <br>Start comparing now
            </p>
          </v-flex>

          <v-flex
            mb-5
            xs12
          >
            <h2 class="headline font-weight-bold mb-3">What's next?</h2>

            <v-layout justify-center>
              <v-card
                class="mx-auto"
                color="#26c6da"
                dark
                max-width="400"
              >
                <v-card-title>
                  <v-icon medium dark>Compare</v-icon>
                </v-card-title>

                <v-row
                  class="lg-6"
                  no-gutters
                >
                  <v-col class="d-flex" cols="4" lg="1">
                  </v-col>
                  <v-col class="d-flex" cols="4" lg="2">
                    <p>Type</p>
                  </v-col>
                  <v-col class="d-flex" cols="4" lg="8">
                    <v-select
                      :items="items"
                      label="Select type"
                      dense
                      solo
                    ></v-select>
                  </v-col>
                  <v-col class="d-flex" cols="4" lg="1">
                  </v-col>
                </v-row>

                <v-row
                  class="lg-6"
                  no-gutters
                >
                  <v-col class="d-flex" cols="4" lg="1">
                  </v-col>
                  <v-col class="d-flex" cols="4" lg="2">
                    <p>Age</p>
                  </v-col>
                  <v-col class="d-flex" cols="4" lg="8">
                    <v-select
                      :items="ages"
                      label="Select age group"
                      dense
                      solo
                    ></v-select>
                  </v-col>
                  <v-col class="d-flex" cols="4" lg="1">
                  </v-col>
                </v-row>

                <v-card-actions>
                  <v-list-tile class="grow">
                    <v-list-tile-avatar color="grey darken-3">
                      <v-flex xs12>
                        <v-img
                          :src="require('../assets/logo.png')"
                          class="my-3"
                          contain
                          height="200"
                        ></v-img>
                      </v-flex>
                    </v-list-tile-avatar>

                    <v-list-tile-content>
                      <v-list-tile-title>Waleed: Proxima Apps</v-list-tile-title>
                    </v-list-tile-content>

                    <v-layout
                      align-center
                      justify-end
                    >
                      <v-icon class="mr-1">mdi-heart</v-icon>
                      <span class="subheading mr-2">256</span>
                      <span class="mr-1">·</span>
                      <v-icon class="mr-1">mdi-share-variant</v-icon>
                      <span class="subheading">45</span>
                    </v-layout>
                  </v-list-tile>
                </v-card-actions>
              </v-card>
            </v-layout>
          </v-flex>

          <v-flex
            xs12
            mb-5
          >
            <h2 class="headline font-weight-bold mb-3">Important Links</h2>

            <v-layout justify-center>

            </v-layout>
          </v-flex>

          <v-flex
            xs12
            mb-5
          >
            <h2 class="headline font-weight-bold mb-3">Ecosystem</h2>

            <v-layout justify-center>

            </v-layout>
          </v-flex>
        </v-layout>
      </v-col>
      <v-col
        :key="3"
        :cols="2"
      >
        <v-card
          class="pa-2"
          outlined
          tile
        >
          <v-img
            :src="require('../assets/logo.svg')"
            class="my-3"
            contain
            height="200"
          ></v-img>
        </v-card>
      </v-col>
    </v-row>

  </v-container>
</template>

<script>
export default {
  name: 'HelloWorld',

  data: () => ({
    items: ['Home', 'Car', 'Content', 'Life'],
    ages: ['1-12', '13-22', '23-40', '41-60'],
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
        href: 'https://madewithvuejs.com/vuetify'
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
        href: 'https://vuetifyjs.com/components/api-explorer'
      },
      {
        text: 'Select a layout',
        href: 'https://vuetifyjs.com/layout/pre-defined'
      },
      {
        text: 'Frequently Asked Questions',
        href: 'https://vuetifyjs.com/getting-started/frequently-asked-questions'
      }
    ]
  })
}
</script>
