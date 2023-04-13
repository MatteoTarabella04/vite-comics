<script>

import appHeader from './components/_header.vue';
import appMain from './components/_main.vue';
import sectionIconBar from './components/_iconBar.vue';
import appFooter from './components/_footer.vue';

export default {
  components: {
    appHeader,
    appMain,
    sectionIconBar,
    appFooter,
  }

}
</script>

<template>
  <appHeader />

  <appMain />

  <sectionIconBar />

  <appFooter />
</template>


<style lang="scss" scoped></style>