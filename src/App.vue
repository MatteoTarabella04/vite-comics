<script>

import appHeader from './components/_header.vue';
import appMain from './components/_main.vue';

export default {
  components: {
    appHeader,
    appMain
  },

  data() {
    return {

    }
  }
}
</script>

<template>
  <appHeader />

  <appMain />

  <footer></footer>
</template>


<style lang="scss" scoped></style>