<template>
  <v-form 
    ref="form"
    v-model="valid"
    lazy-validation
  >
    <v-container class="font-display">
      <v-row align="center" justify="center">
        <v-img
          max-height="95"
          max-width="300"
          :src="require ('../assets/silas.png')"

        ></v-img>    
      </v-row>
      <v-row class="pt-5">
        <v-col cols="12" class="pa-0  font-weight-black mb-1 animate__animated animate__slideInDown">Email</v-col>
        <v-col cols="12"  class="pa-0"> 
          <v-text-field
          v-model='login.email'
          :rules="rules.email"
          color="#38A169"
          outlined
          single-line
          full-width
          height="40"
          hide-details
          class="input-border animate__animated animate__slideInDown"
          
          >
          </v-text-field>
        </v-col>
      </v-row>
      <v-row class="pt-8">
        <v-col cols="12"  class="pa-0 font-weight-black mb-1 animate__animated animate__slideInDown">Senha</v-col>
        <v-col cols="12"  class="pa-0"> 
          <v-text-field
          v-model='login.password'
          :rules="rules.password"
          :type="show1 ? 'text' : 'password'"
          :append-icon="show1 ? 'mdi-eye' : 'mdi-eye-off'"
          color="#38A169"
          outlined
          single-line
          full-width
          height="40"
          hide-details
          @click:append="show1 = !show1"
          class="input-border animate__animated animate__slideInDown"
          >
 
          </v-text-field>
        </v-col>
      </v-row>
    
      <v-row class="pt-8">
        <v-col cols="12"  class="pa-0">
          <v-btn style="border-radius:5px;"
            @click="validationForm"
            class="white--text animate__animated animate__slideInDown"
            color="#38a169"
            height="40"
            block>
            Entrar
          </v-btn>
        </v-col>
      </v-row>
      
      <v-row class="pt-3">
          <v-btn style="border-radius:5px;"
            @click="validationForm"
            class="white--text animate__animated animate__slideInDown"
            color="primary"
            
            height="40"
            block
            href="forgotPassword">
            Esqueceu sua senha?
          </v-btn>
          
      </v-row>
    </v-container>
  </v-form>
</template>
<script>
  import'animate.css';

export default {


  layout: 'login',
    data(){
    return{
      valid: true,
      show1:false,
      login:{
        email:'',
        password:''
      },
      error:false,
      rules:{
          email:[
            v => !!v || 'email  obrigatório',
            this.validateEmail
          ],
          password:[
            v => !!v || 'senha  obrigatória'
           
          ]
        }
    }
  },
 
  }

</script>

<style scoped>
.font-display {
  font-family: 'Poppins' sans-serif;
  

} 

  



</style>