<template>
  <v-container class="container-fluid">
      <div class="row">
        <div class="col col-md-6">
          <div class="h-100 rounded-3">
            <v-img :src="require('../assets/logo.svg')" class="my-3" contain height="500" />
          </div>
        </div>

        <div class="col col-md-6">
            <div class="d-flex align-center justify-center" style="height: 100vh">
              <v-sheet width="350" class="mx-auto">
                  <v-form fast-fail @submit.prevent="login">
                      <v-text-field variant="outlined" v-model="username" label="Usuario"></v-text-field>

                      <v-text-field variant="outlined" v-model="password" label="Contrasena"></v-text-field>
                      <a href="#" class="text-body-2 font-weight-regular">Olvidó su contrasena?</a>

                      <v-btn type="submit" color="orange" block class="mt-2">Ingresar</v-btn>
                  </v-form>
                  <div class="mt-2">
                      <p class="text-body-2">No cuenta con un usuario? <a href="#">Contactar</a></p>
                  </div>
              </v-sheet>
            </div>
          </div>
        </div>

      
  </v-container>
</template>

<script>
  export default {
    name: 'LoginUser',

    data: () => ({
      ecosystem: [
        {
          text: 'vuetify-loader',
          href: 'https://github.com/vuetifyjs/vuetify-loader',
        },
        {
          text: 'github',
          href: 'https://github.com/vuetifyjs/vuetify',
        },
        {
          text: 'awesome-vuetify',
          href: 'https://github.com/vuetifyjs/awesome-vuetify',
        },
      ],
      importantLinks: [
        {
          text: 'Documentation',
          href: 'https://vuetifyjs.com',
        },
        {
          text: 'Chat',
          href: 'https://community.vuetifyjs.com',
        },
        {
          text: 'Made with Vuetify',
          href: 'https://madewithvuejs.com/vuetify',
        },
        {
          text: 'Twitter',
          href: 'https://twitter.com/vuetifyjs',
        },
        {
          text: 'Articles',
          href: 'https://medium.com/vuetify',
        },
      ],
      whatsNext: [
        {
          text: 'Explore components',
          href: 'https://vuetifyjs.com/components/api-explorer',
        },
        {
          text: 'Select a layout',
          href: 'https://vuetifyjs.com/getting-started/pre-made-layouts',
        },
        {
          text: 'Frequently Asked Questions',
          href: 'https://vuetifyjs.com/getting-started/frequently-asked-questions',
        },
      ],
    }),
  }
</script>
