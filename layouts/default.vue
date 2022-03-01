<template>
  <v-app class="app">
    <!-- <navDrawer /> -->
    <Navbar /> 
    <v-main>
        <nuxt />
    </v-main>
  </v-app>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'
import Navbar from '@/components/NavBar.vue'

@Component({
  components: {
    Navbar
  },
})

export default class PrincipalPage extends Vue {
  drawer = false;

}

</script>

<style>

* {
  font-family: 'OpenSansCondensed-Light', sans-serif;
}

.app{
  background-color: var(--v-background-base) !important
}

</style>
