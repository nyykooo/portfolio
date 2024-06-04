<script>
import Header from './components/Header.vue';
import Body from './components/Body.vue';
import Footer from './components/Footer.vue';

export default {
  components: {
    Header,
    Body,
    Footer,
  },
  data() {
    return {
      currentComponent: 'AboutMe',
    };
  },
  methods: {
    changeComponent(componentName) {
      this.currentComponent = componentName;
    },
  },
};
</script>

<style src="./assets/css/app.css"></style>

<template>
  <div class="app">
    <Header @change-component="changeComponent" />
    <Body :current-component="currentComponent" />
    <Footer />
  </div>
</template>
