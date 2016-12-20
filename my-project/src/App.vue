<template>
  <div id="app">
    <intro></intro>
    <main>
      <project-group v-for="projectGroup in projects"
                     v-bind:class="{ open: isOpen }"
                     v-on:click="toggleOpen()"
                     :projectGroup="projectGroup"></project-group>
      <!-- <resume v-bind:class="{ open: isOpen }"
              v-on:click="toggleOpen()"></resume> -->
    </main>
  </div>
</template>

<script>
import Intro from './components/Intro'
import ProjectGroup from './components/ProjectGroup'
import Resume from './components/Resume'

export default {
  data () {
    return {
      projects: {
        section1: {
          sectionName: {title: 'Work'},
          project1: {name: 'Wyzant', id: 'wyzant', category: 'Web Development', tagged: 'product', projectLink: '#'},
          project2: {name: 'Jeni\'s Splendid Ice Creams', id: 'jenis', category: 'iPhone / Android App Development | Design', projectLink: '#'},
          project3: {name: 'Firestone Tire', id: 'firestone', category: 'Web Development', tagged: 'client', projectLink: '#'},
          project4: {name: 'Bridgestone Tire', id: 'bridgestone', category: 'Web Development', tagged: 'client', projectLink: '#'},
          project5: {name: 'Atlanta Humane Society', id: 'ahs', category: 'Web Development | Design', tagged: 'student', projectLink: '#'},
          project6: {name: 'Google Maps / Bandsintown API Integration ', id: 'google', category: 'Web Development', tagged: 'student', projectLink: '#'},
          project7: {name: 'Kotori', id: 'kotori', category: 'Web Game Development', tagged: 'student', projectLink: '#'},
          project8: {name: 'Codepen Projects', id: 'codepen', category: 'Web Development | Design', tagged: 'student', projectLink: '#'}
        }
        // section2: {
        //   sectionName: {title: 'Old Work'},
        //   project1: {name: 'Atlanta Humane Society', id: 'ahs', category: 'Web Development | Design', projectLink: '#'},
        //   project2: {name: 'Google Maps / Bandsintown API Integration ', id: 'google', category: 'Web Development', projectLink: '#'},
        //   project3: {name: 'Kotori', id: 'kotori', category: 'Web Game Development', projectLink: '#'}
        // }
      },
      isOpen: false
    }
  },
  methods: {
    toggleOpen: function () {
      this.isOpen = !this.isOpen
    }
  },
  components: {
    Intro,
    ProjectGroup,
    Resume
  }
}
</script>

<style lang="scss">
body {
  box-sizing: border-box;
  margin: 0 auto;
  padding: 0;
  background: #fdf8f3;
}
h1 {
  font-family: "Open Sans", sans-serif;
  text-transform: uppercase;
  padding: 0 0 .25em;
  font-size: 30px;
  margin: 0;
}
h2 {
  font-family: 'Gentium Basic', serif;
  font-weight: 400;
  padding: 0 0 .25em;
  font-size: 25px;
  letter-spacing: 1.2px;
}
p {
  font-family: "Open Sans", sans-serif;
  margin: .1em;
  font-size: 14px;
  padding: 0 0 1.5em;
  letter-spacing: .4px;
  &:last-of-type {
      padding: 0;
  }
}
a {
  text-decoration: none;
}
</style>
