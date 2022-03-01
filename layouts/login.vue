<template>
  <v-app light class="bg-login">

    <v-main class="d-flex align-content-center flex-wrap">
      <v-container  fluid class=" container-personalisado py-8 px-10 animate__animated animate__pulse" >
           <Nuxt />
      </v-container>
    </v-main>
  </v-app>
</template>
<style scoped>
.container-personalisado{
  width: 100%;
  max-width: 400px !important;
    background-image: linear-gradient(to left,#01C195, #53FFD8, #8EFDFF);
  border-radius:10px;
  box-shadow: 0 0 1em;
}

.bg-login
{

}
</style>
 <script lang="ts">
 import Vue from 'vue'
import login from '~/pages/login.vue';
 import'animate.css';

 export default Vue.extend({

 })
 </script>
