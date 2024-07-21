<template>
  <ul>
    <learning-rosource
      v-for="res in storedResource"
      :key="res.id"
      :title="res.title"
      :description="res.description"
      :link="res.link"
    ></learning-rosource>
  </ul>
</template>

<script>
import LearningRosource from './components/learning-resources/LearningResource.vue';

export default {
  components: {
    LearningRosource,
  },
  data() {
    return {
      storedResource: [
        {
          id: 'official-guide',
          title: 'Official Guide',
          description: 'The official Vue.js documentation',
          link: 'https://vuejs.org',
        },
        {
          id: 'google',
          title: 'Google',
          description: 'The official Vue.js documentation',
          link: 'https://vuejs.org',
        },
      ],
    };
  },
};
</script>
