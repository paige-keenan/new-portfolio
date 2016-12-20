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
    },
    isOpen: {
      type: Boolean
    },
    title: {
      type: Object
    }
  },

  components: {
    Project
  }
}
</script>
<style lang="scss">
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
@media screen and (min-width: 680px) {
    .project-container {
        position: relative;
        header {
            width: 250px;
        }
        main {
            position: absolute;
            right: 0;
            top: 0;
            width: calc(100% - 250px);
            display: flex;
            max-width: 1200px;
            flex-wrap: wrap;
            justify-content: space-around;
            // align-items: flex-start;
            align-items: center;
            // hacky af
            // TODO: not this.
            a:first-child {
                display: none;
            }
            a {
                width: 100%;
            }
        }
    }
}
@media screen and (min-width: 1000px) {
    .project-container {
        main {
            padding: 5em 0;
            a {
                width: 45%;
                min-width: 0;
                margin-right: 1em;
                margin-bottom: 3em;
                box-shadow: 0 14px 22px rgba(0, 0, 0, 0), 0 10px 10px rgba(0, 0, 0, 0.17);
            }
        }
    }
}
@media screen and (min-width: 1400px) {
    .project-container {
        main {
            padding: 5em 0;
            a {
                width: 350px;
                min-width: 350px;
                margin-right: 2em;
                margin-bottom: 3em;
            }
        }
    }
}
</style>
