<template>
    <div class="project-container">
      <header>
        <button>{{ projectGroup.sectionName.title }}</button>
      </header>
      <main>
        <project v-for="project in projectGroup"
                 :project="project"></project>
      </main>
  </div>
</template>

<script>
import Project from './Project'

export default {
  props: {
    projectGroup: {
      type: Object,
      required: true
    }
  },

  components: {
    Project
  }
}
</script>
<style>
button {
    width: 100%;
    font-size: 20px;
    text-align: left;
    font-family: "Open Sans", sans-serif;
    font-weight: 800;
    text-transform: uppercase;
    border: 0;
    background: #f7f3f0;
    padding: 15px 0 15px 50px;
    border-top: 1px solid #ccc;
    letter-spacing: 1.4px;
}
</style>
