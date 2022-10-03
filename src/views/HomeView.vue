<template>
  <div class="home">
    <StyleGuide msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import StyleGuide from '@/components/StyleGuide/index.vue'

export default {
  name: 'HomeView',
  components: {
    StyleGuide
  }
}
</script>
