<script>
import AboutMe from './AboutMe.vue';
import Projects from './Projects.vue';
import Contact from './Contact.vue';

export default {
  props: ['currentComponent'],
  components: {
    AboutMe,
    Projects,
    Contact,
  },
};
</script>

<template>
    <div>
        <AboutMe v-if="currentComponent === 'AboutMe'" />
        <Projects v-if="currentComponent === 'Projects'" />
        <Contact v-if="currentComponent === 'Contact'" />
    </div>
</template>