<template>
  <div class="navbar-props">
    <div class="container-props">

      <NuxtLink to="/">
        <v-img class="animate__animated animate__bounce animate__repeat-2"
          max-height="200"
          max-width="180"
          alt="silas"
          to="/"
         :src="require ('../assets/silas.png')"

        />
      </NuxtLink>

      <!-- menu -->
      <div style="display: flex">

        <!-- home -->
        <v-btn rounded
          class="icon-menu" 
          text
          to="/"
        >
          <span class="text "> Home </span>
          <v-icon >mdi-home</v-icon>
        </v-btn>

        <!-- profile -->
        <v-btn rounded
          class="icon-menu" 
          text
          to="/profile"
        >
          <span class="text"> Perfil </span>
          <v-icon >mdi-account</v-icon>
        </v-btn>

        <!-- exit -->
        <v-btn rounded class="icon-menu" text>
          <span class="text"> Sair </span>
          <v-icon >mdi-logout</v-icon>
        </v-btn>

        
      </div>
    </div>
    
  </div>

</template>

<script lang="ts">
import { Component, Vue } from "nuxt-property-decorator";

@Component({
  components: {},
})
export default class NavBar extends Vue {

 
  }





</script>


<style scoped >

.navbar-props {
  display: flex;
  background-image: linear-gradient(to left,#BDEFFF, #BDEFFF,  #F3FCFE);

  border-bottom: 1px solid #BDEFFF;
  justify-content: center;
  box-shadow: 0 0 1em;
}

.container-props {
  width: 80vw;

  display: flex;
  align-items: center;
  justify-content: space-around;
}

.icon-menu {
  margin-right: 1.2rem;
  font-weight:bold ;
  font-size: 1rem;
  background-image: linear-gradient(to left,#BDEFFF, #BDEFFF,  #F3FCFE);
  color:#074446;


}

</style>
  
</template>

<script>
export default {

}
</script>

<style>

</style>