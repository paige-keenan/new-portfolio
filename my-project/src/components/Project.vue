<template>
  <a href="#">
    <figure :id="project.id"></figure>
    <figcaption>
      <h3>{{ project.name }}</h3>
      <p>{{ project.category }}</p>
    </figcaption>
  </a>
</template>

<script>
export default {
  props: {
    project: {
      type: Object,
      required: true
    }
  }
}
</script>

<style lang="scss">
#wyzant {
  background: url('../assets/wyzant-hero.jpg') center right;
  background-size: cover;
  @media screen and (min-width: 1000px) {
    height: 350px;
  }
}
#firestone {
  background: url('../assets/firestone-hero.jpg') right center;
  background-size: cover;
  @media screen and (min-width: 1000px) {
    height: 250px;
  }
}
#bridgestone {
  background: url('../assets/bridgestone-hero.jpg') center bottom;
  background-size: cover;
  @media screen and (min-width: 1000px) {
    height: 350px;
  }
}
#jenis {
  background: url('../assets/jenis-hero.jpg') center center;
  background-size: cover;
}
#ahs {
  background: url('../assets/humane-society-hero.jpg') center center;
  background-size: cover;
  @media screen and (min-width: 1000px) {
    height: 280px;
  }
}
#google {
  background: url('../assets/maps-hero.jpg') center center;
  background-size: cover;
}
#kotori {
  background: url('../assets/kotori-hero.jpg') center center;
  background-size: cover;
  @media screen and (min-width: 1000px) {
    height: 250px;
  }
}
#codepen {
    background: url('../assets/codepen-hero.jpg') center center;
    background-size: cover;
    @media screen and (min-width: 1000px) {
      height: 350px;
    }
}
figure {
  width: 100%;
  height: 425px;
  margin: 0;
}
figcaption {
  padding: 1em 1em 2em;
  h3 {
    color: #000;
    margin: 0;
    font-size: 20px;
    letter-spacing: 1.4px;
    font-weight: 800;
    margin-bottom: 5px;
  }
  p {
    color: #000;
    font-size: 12px;
    margin: 0;
  }
}
</style>
