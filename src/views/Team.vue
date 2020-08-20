<template>
  <div class="team">
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
            <li>Project Deadline : 10-June-2020</li>
          </ul>
        </div>
      </v-layout>
    </v-container>
    <v-divider width="92%" class="line-rule"></v-divider>
    <CardList />
  </div>
</template>

<script>
// @ is an alias to /src
import CardList from '@/components/CardList.vue'
export default {
  name: "team",
  components: {
   CardList,
  },
  data: () => ({}),
};
</script>
<style scoped>

li {
  display: inline-block;
  padding: 0px 20px;
}
.flex-card {
  display: flex;
  justify-content: space-between;
}
@media (max-width: 768px) {
  
  .team{
  overflow-x: scroll;
}
}
</style>
