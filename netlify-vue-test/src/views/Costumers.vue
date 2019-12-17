<template>
  <div class="table">
    <div class="display-4 d-flex justify-center">
      Project Overview
    </div>

    <h1>HELLO</h1>

    <v-data-table :items="projects" :headers="headers"> </v-data-table>
    <div class="d-flex flex-wrap">
      <div v-for="project in proejcts" :key="project.name">
        <ProjectListProject
          :project="project"
          :tags="tags"
        ></ProjectListProject>
      </div>
    </div>
  </div>
</template>

<script>
//import { mapstate } from 'vuex';
import ProjectListProject from "../components/Table";
export default {
  components: {
    ProjectListProject
  },
  compupet: {
    headers() {
      return [
        { text: "Project name", value: "name" },
        { text: "Time spent", value: "time" },
        { text: "Project status", value: "status" },
        { text: "Client connection", value: "client" }
      ];
    }
  }
};
</script>
