<template>
    <div class="title">
        <h1>Projects</h1>
    </div>
    <Projects/>
</template>
<script>
import Projects from '@/components/Project.vue'
export default {
  name: 'ProjectView',
  components: {
    Projects
  }
  }
</script>