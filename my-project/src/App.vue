<template>
  <div id="app">
    <intro></intro>
    <main>
      <project-group v-for="projectGroup in projects"
                     :projectGroup="projectGroup"></project-group>
      <resume></resume>
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
          sectionName: {title: 'New Work'},
          project1: {name: 'Wyzant', id: 'wyzant', category: 'Web Development', projectLink: '#'},
          project2: {name: 'Jeni\'s Splendid Ice Creams', id: 'jenis', category: 'iPhone / Andriod App Development, Design', projectLink: '#'},
          project3: {name: 'Firestone Tire', id: 'firestone', category: 'Web Development', projectLink: '#'},
          project4: {name: 'Bridgestone Tire', id: 'bridgestone', category: 'Web Development', projectLink: '#'}
        },
        section2: {
          sectionName: {title: 'Old Work'},
          project1: {name: 'Atlanta Humane Society', id: 'ahs', category: 'Web Development, Design', projectLink: '#'},
          project2: {name: 'Google Maps / Bandsintown API Integration ', id: 'google', category: 'Web Development', projectLink: '#'},
          project3: {name: 'Kotori', id: 'kotori', category: 'Web Game Development', projectLink: '#'}
        }
      }
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
