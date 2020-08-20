<template>
  <v-container>
    <v-layout row wrap>
      <v-flex class="section">
        <ModuleCard />
        <div class="column4">
          <div class="text-icon">
            <h4 class="pl-4">Make the background image blur</h4>
            <div class="my-2">
              <v-btn class="pass" dark width="50px">Pass</v-btn>
            </div>
          </div>
          <div class="text-icon">
            <h4 class="pl-4">Apply gredient colours on the navigation</h4>
            <div class="my-2">
              <v-btn class="pass" dark width="50px">Pass</v-btn>
            </div>
          </div>
          <div class="text-icon">
            <h4 class="pl-4">Make the background image blur</h4>
            <div class="my-2">
              <v-btn class="pass" dark width="50px">Pass</v-btn>
            </div>
          </div>
          <div class="text-icon">
            <h4 class="pl-4">Apply gredient colours on the navigation</h4>
            <div class="my-2">
              <v-btn class="pass" dark width="50px">Pass</v-btn>
            </div>
          </div>
          <div class="text-icon">
            <h4 class="pl-4">Make the background image blur</h4>
            <div class="my-2">
              <v-btn class="pass" dark width="50px">Pass</v-btn>
            </div>
          </div>
          <div class="text-icon">
            <h4 class="pl-4">Make the background image blur</h4>
            <div class="my-2">
              <v-btn class="pass" dark width="50px">Pass</v-btn>
            </div>
          </div>
          <div class="text-icon">
            <h4 class="pl-4">Apply gredient colours on the navigation</h4>
            <div class="my-2">
              <v-btn class="pass" dark width="50px">Pass</v-btn>
            </div>
          </div>
          <div class="text-icon">
            <h4 class="pl-4">Make the background image blur</h4>
            <div class="my-2">
              <v-btn class="pass" dark width="50px">Pass</v-btn>
            </div>
          </div>
          <div class="text-center">
            <v-btn class="ma-2 " tile id="btn-indigo">New Test Case</v-btn>
            <v-btn class="ma-6" width="40%" tile outlined color="normal">
               Test
            </v-btn>
            <!-- <v-btn class="ma-2" tile large color="teal" icon>
              <v-icon>mdi-vuetify</v-icon>
            </v-btn> -->
          </div>
        </div>
        <!-- added test case -->
        <!-- <h3>Modules</h3> -->
        <div class="column6 text-center">
          <div id="column">
            <div class="card-red">
              <div class="text-icon">
                <v-icon color="white " class="icons">mdi-briefcase</v-icon>
                <h4>20</h4>
              </div>
              <p>Total Modules</p>
            </div>
            <div class="card-black">
              <div class="text-icon">
                <v-icon color="white " class="icons">mdi-briefcase</v-icon>
                <h4>20</h4>
              </div>
              <p>Improvement</p>
            </div>
          </div>

          <div class="container">
            <div class="card-blue">
              <div class="text-icon">
                <v-icon color="white " class="icons">mdi-briefcase</v-icon>
                <h4>20</h4>
              </div>
              <p>Total Modules test</p>
            </div>
            <div class="card-pink">
              <div class="text-icon">
                <v-icon color="white " class="icons">mdi-briefcase</v-icon>
                <h4>20</h4>
              </div>
              <p>Total failed</p>
            </div>
          </div>
          <div class="container">
            <div class="card-green">
              <div class="text-icon">
                <v-icon color="white" class="icons">mdi-briefcase</v-icon>
                <h4>20</h4>
              </div>
              <p>Total passed</p>
            </div>
            <div class="card-purple">
              <div class="text-icon">
                <v-icon color="white" class="icons">mdi-briefcase</v-icon>
                <h4>20</h4>
              </div>
              <p>Total Untested</p>
            </div>
          </div>
        </div>
        <!-- <div class="column4 text-center"></div>
          <div class="column4 text-center"></div> -->
      </v-flex>
    </v-layout>
  </v-container>
</template>
<script>
import ModuleCard from "@/components/ModuleCard.vue";
export default {
  components: {
    ModuleCard,
  },
};
</script>
<style scoped>
.card-section {
  display: flex;
  justify-content: space-around;
}
#column {
  display: flex;
  justify-content: space-around;
}
.container {
  display: flex;
  justify-content: space-around;
}
.card-red,
.card-blue,
.card-pink,
.card-black,
.card-green,
.card-purple,
.card-red {
  margin-top: 20px;
  width: 40%;
  height: 112px;
  box-shadow: 0px 0px 2px rgba(0, 0, 0, 0.15);
  border-radius: 5px;
  color: white;
}
.icons {
  background-color: gray;
  width: 40px;
  height: 40px;
  border-radius: 50px;
  opacity: 0.5;
}
p {
  font-size: 13px;
  padding-top: 30px;
  padding-right: 20px;
}

.column6 {
  background-color: #ffffff;
  width: 90%;
  margin: 20 0px;
}
.column4 {
  background-color: #ffffff;
  width: 100%;
  height: 35rem;
  margin: 20px;
}
.section {
  display: flex;
  justify-content: space-around;
}
.card-red {
  background-color: #f15832;
  padding: 5px 20px;
}
.card-black {
  background: rgba(3, 41, 61, 0.8);
  padding: 5px 20px;
}
.card-blue {
  background: #296799;
  padding: 5px 20px;
}
.card-pink {
  background: #f8426e;
  padding: 5px 20px;
}
.card-green {
  background: #4dbd98;
  padding: 5px 20px;
}
.card-purple {
  background: #3d43a2;
  padding: 5px 20px;
}
.text-icon {
  display: flex;
  justify-content: space-between;
}
.line-rule {
  margin-left: 70px;
}
.pass {
  background: linear-gradient(0deg, #4dbd98, #4dbd98),
    linear-gradient(0deg, #4dbd98, #4dbd98),
    linear-gradient(0deg, #4dbd98, #4dbd98), #4dbd98;
  /* margin-left: 80px; */
}
h4 {
  font-size: 14px;
  color: #03293d;
}
#btn-indigo{
  background-color: #23B3E8;
  color: white;
}
@media (max-width: 768px) {
  /* .section {
    flex-direction: column;
  } */
  .column4 {
    background-color: #ffffff;
    width: 90%;
    height: 25rem;
    margin: 20px;
  }
}
</style>
