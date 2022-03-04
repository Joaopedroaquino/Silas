
<template>
<v-app class="all">
  <div class="content">
    <v-row cols="12" sm="8" md="6">
      <NuxtLink to="/silascast" style="text-decoration: none">
        <div class="buttom-details1">
          <div class="menu-button-details" type="button">
            <v-icon class="icons-menu-details animate__animated animate__heartBeat animate__infinite infinite" color="white" size="90px"
              >mdi-microphone</v-icon
            >
          </div>
          <span style="text-decoration: none" class="title-details1"></span>
        </div>
      </NuxtLink>

      <NuxtLink to="/silaskey" style="text-decoration: none">
        <div class="buttom-details2">
          <div class="menu-button-details" type="button">
            <v-icon class="icons-menu-details  animate__animated animate__rotateIn animate__infinite infinite animate__slow	10s" color="white" size="90px "
              >mdi-key-variant</v-icon
            >
          </div>
          <a href="/access" style="text-decoration: none" class="title-details2"
            ></a
          >
        </div>
      </NuxtLink>

       <NuxtLink to="/silascar" style="text-decoration: none">
        <div class="buttom-details2">
          <div class="menu-button-details" type="button">
            <v-icon  class="icons-menu-details animate__animated animate__zoomIn animate__infinite infinite animate__slow	10s" color="white" size="90px"
              >mdi-car-connected</v-icon
            >
          </div>
          <a href="/car" style="text-decoration: none" class="title-detailsC"
            ></a
          >
        </div>
      </NuxtLink>
        <NuxtLink to="/newdashboard" style="text-decoration: none">
        <div class="buttom-details2">
          <div class="menu-button-details" type="button">
            <v-icon  class="icons-menu-details animate__animated animate__fadeOut animate__infinite infinite animate__slow	1s" color="white" size="90px"
              >mdi-alert</v-icon
            >
          </div>
          <a href="/car" style="text-decoration: none" class="title-detailsC"
            ></a
          >
        </div>
      </NuxtLink>

      <NuxtLink to="/dashboard" style="text-decoration: none">
        <div class="buttom-details3">
          <div class="menu-button-details" type="button">
            <v-icon class="icons-menu-details" color="white" size="90px"
              >mdi-monitor</v-icon
            >
          </div>
          <span  style="text-decoration: none" class="title-details3"> </span>
        </div> </NuxtLink
      >
    </v-row>

  
  </div>
</v-app>
</template>


<script lang="ts">
  import'animate.css';

import { Component, Vue } from "nuxt-property-decorator";

@Component({
  components: {},
})
export default class Document extends Vue {


  meetingDetails: boolean = false;

  tab = 0;

  itemsPerPage: number = 5;
  page: number = 1;
  pageCount: number = 0;

  checkSectionForm = false;

}
</script>

<style scoped>


.all {
background-color:#D0F4FF ;
}
.content {
  display: flex;
  align-items: center;
  justify-content: center;
  margin-top: 300px;
  margin-left: 280px;
}

.menu-button-details {
  width: 20vh;
  height: 10vw;
  border-radius: 100px;
  background-image: linear-gradient(to left,#0D4BFE, #0DC3FE, #93AFFF);
  box-shadow: 0 0 1.5em;
  border: solid 0.5px #F4FCFF;
}

.icons-menu-details {
  margin-left: 50px;
  margin-top: 50px;
  color: rgb(215, 13, 241);
  size: 50px;
}

.title-details1 {
  font-size: 24px;
  color: #029d88;
  margin-left: 1rem;
}

.title-details2 {
  font-size: 24px;
  color: #029d88;
  margin-left: 1rem;
}

.title-detailsC {
  font-size: 24px;
  color: #029d88;
  margin-left: 1rem;
}


.title-details3 {
  font-size: 24px;
  color: #029d88;
  margin-left: 1rem;
}

.buttom-details1 {
  margin-left: 120px;
}
.buttom-details2 {
  margin-left: 50px;
}
.buttom-details3 {
  margin-left: 120px;
}
</style>
