<template>
  <div class="team">
    <h1 class="subheading grey--text">Team</h1>
    <v-container>
      <v-layout  class="flex-card">
        <div class="link-text">
          <ul>
            <li>Overview</li>
            <li>Teams</li>
            <li>Modules</li>
            <li>Files</li>
            <li>In Progress</li>
          </ul>
          
        </div>
        <div class="link-text">
            <ul>
            <li>All Task</li>
            <li>All Modules</li>
            <li>Modules</li>
            <!-- <li>Files</li> -->
            <li>Project Deadline :6 weeks</li>
          </ul>
        </div>
      </v-layout>
    </v-container>
    <v-container>
      <v-layout row wrap>
        <v-flex class="section">
          <div class="column5 text-center"><v-icon>mdi-plus</v-icon></div>
          <div class="column5 text-center">2</div>
          <div class="column5 text-center">3</div>
          <div class="column5 text-center">4</div>
          <div class="column5 text-center">5</div>
        </v-flex>
      </v-layout>
      <v-layout row wrap>
        <v-flex class="section">
          <div class="column4 text-center"></div>
          <div class="column4 text-center"></div>
          <div class="column4 text-center"></div>
          <div class="column4 text-center"></div>
          <div class="column4 text-center"></div>
        </v-flex>
      </v-layout>
    </v-container>
    <v-container>
      <v-layout>
        <div class="icon-bg"><v-icon class="icon-plus">mdi-plus</v-icon></div>
      </v-layout>
    </v-container>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "team",
  components: {},
  data: () => ({}),
};
</script>
<style scoped>
.column5 {
  background-color: #FFFFFF;
  width: 60%;
  margin: 20px;
}
.column4 {
  background-color: #FFFFFF;
  width: 60%;
  height: 25rem;
  margin: 20px;
}
.section {
  display: flex;
  justify-content: space-around;
}
.icon-plus{
  background-color: #23B3E8;;
  color: white;
  height: 60px;
  width: 60px;
  text-align: center;
  padding-top: 4px;
  border-radius: 40px;
}
.icon-bg{
   position: relative;
  left: 90%;
  bottom: 50%;
}
li{
  display: inline-block;
  padding: 0px 20px;
}
.flex-card{
  display: flex;
  justify-content: space-between;
}
@media (max-width: 768px) {
  .section {
    flex-direction: column;
  }
}
.team{
  background-color: #F7F7F7;
}
</style>
