<script>
export default {
  methods: {
    showComponent(componentName) {
      this.$emit('change-component', componentName);
    },
  },
};
</script>

<template>
  <div class="header">
    <div @click="showComponent('AboutMe')" class="header_button">About Me</div>
    <div @click="showComponent('Projects')" class="header_button">Projects</div>
    <div @click="showComponent('Contact')" class="header_button">Contact</div>
  </div>
</template>
