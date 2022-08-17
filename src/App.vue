<template>
  <Header/>
  <Introduction/>
  <Experience/>
  <Projects/>
  <Education/>
  <Footer/>
</template>

<script>
import Header from './components/Header.vue';
import Introduction from './components/Introduction.vue';
import Experience from './components/Experience.vue';
import Education from './components/Education.vue';
import Footer from './components/Footer.vue';
import Projects from './components/Projects.vue';

export default {
    components: { Header, Introduction, Experience, Education, Footer, Projects}
}
</script>

<style>
  body {
  font-family: "Fira Sans", Arial, Helvetica, sans-serif;
  margin: 0px;
  color: #141414;
  background-image: url(./assets/img/background1.jpg);
  background-size:  cover;
}

h1,
h2,
h3,
p {
  margin: 0px;
}
ul {
  margin: 0px;
  padding: 0px;
  list-style: none;
}

img {
  max-width: 100%;
  height: auto;
  display: block;
}


.subtitulo {
  font-size: 8rem;
  line-height: 1;
  text-transform: uppercase;
  word-break: break-all;
  max-width: 4ch;
}
@media (max-width: 800px) {
  .subtitulo {
    font-size: 3rem;
    text-transform: capitalize;
    max-width: initial !important;
  }
}

</style>