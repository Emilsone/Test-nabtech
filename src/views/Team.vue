<template>
  <div class="team">
    <h1 class="subheading grey--text">Team</h1>
    <v-container>
      <v-layout class="flex-card">
        <div class="link-text">
          <ul>
            <li>Overview</li>
            <li>Teams</li>
            <li>Text</li>
            <li>Files</li>
            <li>Progress</li>
          </ul>
        </div>
        <div class="link-text">
          <ul>
            <li>All Task</li>
            <!-- <li>All Modules</li>
            <li>Modules</li> -->
            <!-- <li>Files</li> -->
            <li>Project Deadline :10-June-2020</li>
          </ul>
        </div>
      </v-layout>
    </v-container>
    <v-container>
      <!-- <v-layout row wrap>
        <v-flex class="section">
          <div class="column5 text-center"><v-icon>mdi-plus</v-icon></div>
          <div class="column5 text-center">2</div>
          <div class="column5 text-center">3</div>
          <div class="column5 text-center">4</div>
          <div class="column5 text-center">5</div>
        </v-flex>
      </v-layout> -->
      <v-layout row wrap>
        <v-flex class="section">
          <div class="column4 text-center"></div>
          <div class="column4 text-center"></div>
          <div class="column6 text-center" id="column">
            <div class="card-blue" >
              good
            </div>
            <div class="card-red">
              good
            </div>
          </div>
          <!-- <div class="column4 text-center"></div>
          <div class="column4 text-center"></div> -->
        </v-flex>
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
.card-section {
  display: flex;
  justify-content: space-around;
}
#column{
  display: flex;
  justify-content: space-around;
}
.card-red ,.card-blue {
  width: 20%;
  background-color: black;
  height: 20px;
}
li {
  display: inline-block;
  padding: 0px 20px;
}
.flex-card {
  display: flex;
  justify-content: space-between;
}
.column6 {
  background-color: #FFFFFF;
  width: 90%;
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
</style>
