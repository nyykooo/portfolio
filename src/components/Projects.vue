
<template>
  <div>
    <div class="projects">
      <div class="projects__buttons" @click="showProject('Fdf')">Fdf</div>
      <div class="projects__buttons" @click="showProject('PushSwap')">PushSwap</div>
      <div class="projects__buttons" @click="showProject('Minitalk')">Minitalk</div>
    </div>
    <div class="details">
      <Fdf v-if="currentProject === 'Fdf'" />
      <PushSwap v-if="currentProject === 'PushSwap'" />
      <Minitalk v-if="currentProject === 'Minitalk'" />
    </div> 
  </div>
</template>
  
<script>
import Fdf from './projects/Fdf.vue';
import PushSwap from './projects/PushSwap.vue';
import Minitalk from './projects/Minitalk.vue';

export default {
  components: {
    Fdf,
    PushSwap,
    Minitalk,
  },
  data() {
    return {
      currentProject: null,
    };
  },
  methods: {
    showProject(projectName) {
      if (this.currentProject === projectName) {
        this.currentProject = null;
      } else {
        this.currentProject = projectName;
      }
    },
  },
};
</script>
  