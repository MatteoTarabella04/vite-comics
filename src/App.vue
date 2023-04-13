<script>

import appHeader from './components/_header.vue';
import appMain from './components/_main.vue';
import sectionIconBar from './components/_iconBar.vue';

export default {
  components: {
    appHeader,
    appMain,
    sectionIconBar,
  },

  data() {
    return {

    }
  },

}
</script>

<template>
  <appHeader />

  <appMain />

  <sectionIconBar />


  <footer></footer>
</template>


<style lang="scss" scoped></style>