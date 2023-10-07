<template>
  <section class="home-page">
    <div class="intro">

      <h1>Hello and Welcome!</h1>
      <p>Welcome to my portfolio website! Feel free to look around and see previous projects (1.1P and 1.2P), and also find out more about me!</p>
      <button @click="showProjects" class="projectButton">View My Projects</button>
    </div>
    <div class="project-list" v-if="projectsVisible">
      <h2 style="text-align:center">My Tasks</h2>
      <table>
        <tr>
          <th>Link</th>
          <th>Preview</th>
          <th>Description</th>
        </tr>
        <tr>
          <th> <a href="https://github.com/knightjai1/1.1P" target="_blank">Pass Task 1.1P</a> </th>
          <th> <img src="../assets/img1-1P.png" class="projectImage"> </th>
          <th> <p>This pass task was an introduction to HTML and CSS Web Development. 
            The task requirements were to have different HTML tags, such as img and table, 
            as well as include inline CSS formatting and external formatting.</p> </th>
        </tr>
        <tr>
          <th> <a href="https://github.com/knightjai1/SIT1201.2PJai" target="_blank">Pass Task 1.2P </a> </th>
          <th> <img src="../assets/img1-2P.png" class="projectImage"> </th>
          <th> This pass task was a further implementation of the prior pass task, 
            however we had to explore the concept of Responsive Web Apps, and how to integrate that into our website. 
            Additionally, the concept of JavaScript scripting was introduced in this task, 
            and had to include a variety of methods using scripts.</th>
        </tr>
      </table>
    </div>
  </section>
</template>

<script setup>
  import { ref } from 'vue';

  const projectsVisible = ref(false);

  const showProjects = () => {
    projectsVisible.value = true;
  };
</script>

<style>
</style>